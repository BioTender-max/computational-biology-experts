# Frameworks — Núria López-Bigas

## 1. The IntOGen Driver Discovery Pipeline

A multi-method pipeline for identifying cancer driver genes from cohorts of tumor somatic mutations.

**Stage 1 — Input**
Somatic mutation calls from tumor cohorts (whole-exome or whole-genome sequencing). Minimum cohort size: ~100 tumors for reliable driver detection.

**Stage 2 — Background Modeling**
Estimate the expected neutral mutation rate per gene, accounting for:
- Trinucleotide context (the sequence surrounding each mutated base)
- Gene length and expression level
- Replication timing and chromatin accessibility
- Synonymous mutations as a neutral reference

**Stage 3 — Signal Detection (Parallel Methods)**
- **OncodriveFM**: Detects bias toward high-functional-impact mutations (SIFT, PolyPhen, MutationAssessor scores). A gene with more high-impact mutations than expected under neutrality is a candidate driver.
- **OncodriveCLUSTL**: Detects abnormal positional clustering of mutations within the protein sequence. Gain-of-function mutations often cluster in specific functional domains.
- **Oncodrive3D**: Detects clustering in 3D protein structure using AlphaFold models, extending structural analysis to the entire human proteome.
- **dNdScv**: Detects elevated nonsynonymous-to-synonymous mutation ratio (dN/dS > 1 indicates positive selection).

**Stage 4 — Integration**
Combine p-values across methods using a meta-analysis approach. Genes significant in multiple methods are high-confidence drivers. Genes significant in only one method are lower-confidence candidates.

**Stage 5 — Annotation**
- Classify driver genes by role: oncogene vs. tumor suppressor (OncodriveROLE)
- Annotate tissue specificity: pan-cancer vs. cancer-type-specific drivers
- Annotate mechanism: mutation clustering pattern, functional impact type

**Output**
A compendium of cancer driver genes with evidence scores, available at intogen.org. Current version: 568 driver genes across 66 cancer types from 28,000+ tumors.

**Key insight**: No single signal is sufficient. The pipeline's power comes from combining orthogonal signals that capture different mechanisms of positive selection.

---

## 2. BoostDM — In Silico Saturation Mutagenesis

A framework for predicting the driver potential of every possible mutation in every cancer gene.

**Conceptual Foundation**
Thousands of tumors have collectively tested the oncogenic potential of millions of mutations. These natural experiments can train machine learning models that generalize to untested mutations — achieving what experimental saturation mutagenesis does for individual genes, but computationally, across all cancer genes.

**Implementation**
For each cancer gene × tissue combination:
1. Collect all observed somatic mutations in that gene across tumor cohorts
2. Label mutations as driver (positive selection signal) or passenger (neutral)
3. Compute features: functional impact scores, evolutionary conservation, mutation clustering, structural context, trinucleotide context
4. Train a gradient boosting model (XGBoost) on labeled mutations
5. Apply the model to all possible mutations in that gene to generate a driver potential score (0–1)

**Output**
"Driver potential blueprints" — for each cancer gene, a map of every possible mutation with its predicted driver probability in each cancer type. Available at intogen.org/boostdm.

**Validation**
BoostDM models outperform experimental saturation mutagenesis in identifying driver vs. passenger mutations (Muiños et al., 2021, *Nature*).

**Clinical Application**
Integrated into CGI to interpret variants of uncertain significance in patient tumors. Converts VUS into actionable driver/passenger classifications.

**Scale**
185 gene-tissue-specific models covering the most recurrent cancer driver genes.

---

## 3. Cancer Genome Interpreter (CGI) — Clinical Mutation Annotation

A tool for translating tumor somatic mutations into clinically actionable information.

**Input**
Somatic mutations from a patient's tumor (VCF or MAF format), plus tumor type.

**Processing Pipeline**
1. **Driver identification**: Match mutations against IntOGen compendium; apply BoostDM models for gene-specific driver scoring
2. **Biomarker annotation**: Match mutations against curated databases of clinical evidence for drug response (FDA-approved therapies, clinical trials, preclinical evidence)
3. **Actionability classification**: Tier mutations by clinical evidence level (approved biomarker → clinical trial → preclinical → biological evidence)

**Output**
A structured report distinguishing driver from passenger mutations, identifying therapeutic targets, and flagging biomarkers for approved or investigational therapies.

**Design Principle**
Interpretable, not a black box — every classification is traceable to specific evidence. Oncologists can understand why a mutation is classified as actionable.

**Use Case**
Supports oncologists in selecting targeted therapies for individual patients. Particularly valuable for rare mutations where clinical experience is limited.

---

## 4. Mutational Landscape Decomposition — From Signatures to Mechanisms

A framework for understanding the mutagenic processes that shaped a tumor's genome.

**Observation**
The pattern of somatic mutations (trinucleotide context, strand bias, genomic distribution) reflects the mutational processes that generated them — UV exposure, tobacco carcinogens, APOBEC activity, defective DNA repair, chemotherapy.

**Method**
1. Decompose the mutation spectrum into known COSMIC signatures using non-negative matrix factorization
2. Map signature activity to chromatin features (replication timing, nucleosome positioning, transcription factor binding)
3. Identify how DNA repair deficiencies alter the mutation landscape
4. Quantify the contribution of each mutational process to the total mutation burden

**Key Findings from López-Bigas Lab**
- Nucleotide excision repair (NER) is impaired at transcription factor binding sites and nucleosome-embedded DNA, creating local mutation hotspots (Sabarinathan et al., 2016, *Nature*)
- Somatic mutation rates exhibit a 10-bp periodicity tracking the DNA minor groove orientation around nucleosomes (Pich et al., 2018, *Cell*)
- Six chemotherapy agents leave distinct mutational footprints in tumor genomes (Pich et al., 2019, *Nature Genetics*)

**Application**
- Identify the mutagenic exposures a patient has experienced
- Quantify treatment-induced mutation burden
- Improve background models for driver detection by accounting for signature-specific mutation rate variation

---

## 5. Clonal Hematopoiesis Driver Discovery — Repurposing Cancer Genomics Methods

Applying cancer driver detection methods to identify genes driving clonal expansion in normal blood tissue.

**Problem**
Clonal hematopoiesis (CH) — the expansion of hematopoietic stem cell clones carrying somatic mutations — is a risk factor for hematologic malignancies and cardiovascular disease. The full compendium of CH driver genes is unknown.

**Approach**
"Reverse calling": use tumor samples as reference to identify blood somatic mutations in 12,000+ cancer patients (from blood/tumor pairs), then apply IntOGen to detect positive selection signals in the blood mutations.

**Why This Works**
The same evolutionary logic applies: CH driver mutations confer a proliferative advantage to hematopoietic stem cells, just as cancer driver mutations confer advantage to tumor cells. The statistical methods are identical.

**Result**
~70 CH driver genes identified, available at intogen.org/ch. Recovers known CH genes (DNMT3A, TET2, ASXL1) and discovers new candidates.

**Principle**
Methods developed for cancer are transferable to any clonal expansion process governed by positive selection. The framework is general; the application is specific.
