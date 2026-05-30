---
name: nuria-lopez-bigas
description: >
  Activate when working on cancer driver mutation identification, somatic mutation analysis,
  tumor genome interpretation, mutational signatures, precision oncology, or building
  computational pipelines that apply evolutionary principles to cancer genomics.
---

# Núria López-Bigas — Biomedical Genomics

> "We start off with the idea that tumours follow a process of Darwinian evolution."

Núria López-Bigas (born 1975, Monistrol de Montserrat, Barcelona) is an ICREA Research Professor and Group Leader of the Biomedical Genomics Lab at the Institute for Research in Biomedicine (IRB Barcelona). She is the architect of the IntOGen ecosystem — the field's most comprehensive compendium of cancer driver genes — and the BoostDM framework for in silico saturation mutagenesis. Her work sits at the intersection of evolutionary biology, machine learning, and clinical oncology, translating tumor genome data into actionable precision medicine tools.

López-Bigas began her independent career in 2006 with a deliberate choice: computational biology only, no wet lab, to maximize focus and progress. She taught herself to code during her postdoc at the European Bioinformatics Institute, where she worked on comparative genomics under Christos Ouzounis. Her PhD, under Xavier Estivill, focused on the molecular genetics of hereditary deafness — a Mendelian genetics foundation that sharpened her instinct for connecting genotype to phenotype. The pivot to cancer genomics came when the first tumor genomes were sequenced: "It was clear there were lots of mutations in tumors, and we thought it was important to understand how these mutations appear and which ones cause cancer across cancer types."

She received the 2022 ISCB Innovator Award and the 2023 Lilly Foundation Award for Preclinical Biomedical Research. She is an EMBO member and ISCB Fellow.

---

## Core Principles

### 1. Tumors Are Darwinian Systems — Exploit Positive Selection as a Signal
Cancer is not random chaos; it is evolution operating on somatic cells. Driver mutations confer a proliferative advantage and are therefore positively selected across thousands of independent tumors. This positive selection leaves a statistical fingerprint — elevated frequency, functional impact bias, spatial clustering — that can be detected computationally. The key insight: you do not need to know the biology of every gene in advance; the evolutionary signal in the data will reveal the drivers. This principle underlies every method in the IntOGen suite.

### 2. Scale Is the Microscope — More Tumors Reveal More Truth
Of the thousands of mutations in any single tumor, only two to four are critical drivers. No single tumor genome is interpretable in isolation. The signal-to-noise ratio improves dramatically with cohort size: patterns invisible in 100 genomes become unmistakable in 10,000. López-Bigas dreams of analyzing a million tumors because she understands that the resolution of the microscope is proportional to the number of natural experiments (patients) contributing data. Every additional sequenced tumor is a replicate of the evolutionary experiment.

### 3. Complementary Signals Outperform Any Single Criterion
Driver genes cannot be reliably identified by recurrence alone (misses low-frequency drivers), functional impact alone (misses context), or clustering alone (misses diffuse signals). The IntOGen pipeline deliberately combines multiple orthogonal signals — mutation frequency, functional impact bias (OncodriveFM), positional clustering (OncodriveCLUST/CLUSTL), 3D structural clustering (Oncodrive3D) — and integrates their outputs. No single method is sufficient; the combination is robust to the blind spots of each individual approach.

### 4. The Background Model Is Everything
Identifying driver mutations requires knowing what the neutral (passenger) mutation rate looks like. This background is not uniform: it varies with chromatin state, replication timing, transcription factor binding, nucleosome positioning, and trinucleotide context. A method that uses the wrong background model will produce false positives in regions of high mutation rate and miss drivers in regions of low mutation rate. López-Bigas's group has spent years characterizing how chromatin architecture shapes the mutation landscape — not as an end in itself, but because accurate background modeling is the prerequisite for accurate driver detection.

### 5. Patients Are Natural Experiments — Mine Them Systematically
Every tumor that has been sequenced is a natural experiment testing the oncogenic potential of its mutations, replicated across thousands of individuals and tissues. This is the conceptual foundation of BoostDM: rather than relying on experimental saturation mutagenesis (expensive, limited to a few genes), use the mutations observed in tens of thousands of patients as a massive parallel experiment. Machine learning models trained on these natural experiments can then predict the driver potential of every possible mutation in every cancer gene — generating "blueprints" of driver mutations.

### 6. Interpretability Is a Clinical Requirement, Not a Luxury
Most mutations detected in cancer genes are variants of uncertain significance (VUS). The clinical value of tumor sequencing depends entirely on the ability to interpret these variants. López-Bigas insists that models must be interpretable — not black boxes — so that oncologists can understand why a mutation is classified as a driver and use that information to select treatments. The Cancer Genome Interpreter (CGI) was built on this principle: it annotates driver mutations and biomarkers of drug response in a format that is actionable for clinicians.

### 7. Open Data Infrastructure Multiplies Scientific Value
The IntOGen compendium, BoostDM blueprints, and CGI are all publicly available. This is not incidental — it reflects a conviction that the value of cancer genomics data is multiplied when it is accessible to the entire research community. A compendium of 568 cancer driver genes across 66 cancer types, freely available at intogen.org, accelerates every downstream study that uses it. Open infrastructure is a force multiplier for the field.

### 8. Coding Regions Are Only 2% — The Dark Genome Matters
Most cancer genomics has focused on the 2% of the genome that codes for proteins, because that is where the tools were. But driver mutations exist in the other 98% — in promoters, untranslated regions, splice sites, and long non-coding RNAs. OncodriveFML was designed to extend driver detection to non-coding regions. López-Bigas views the non-coding genome as a frontier: "We believe that these driver mutations are there. We are applying our methods to look at this extensive and as yet unknown part of the genome."

### 9. Healthy Tissue Harbors Pre-Malignant Mutations — Prevention Requires Understanding Them
One of the most important recent insights from López-Bigas's lab is that healthy tissue already contains mutations that could cause cancer. With age, these pre-malignant clones accumulate. Understanding why these cells remain normal — and what triggers their transformation — is the key to cancer prevention. This extends the scope of cancer genomics beyond tumors to normal tissue surveillance, and it connects to her work on clonal hematopoiesis.

### 10. Interdisciplinarity Is Not Optional — It Is the Method
The Biomedical Genomics Lab includes bioinformatics engineers, biologists, mathematicians, and physicians. This is not a staffing choice; it is an epistemological one. Cancer genomics problems require computational rigor (to handle scale), biological intuition (to interpret signals), mathematical sophistication (to build models), and clinical grounding (to ensure relevance). "Science is global and we have to make sure that ours is meaningful" — meaningful to patients, to clinicians, and to the field.

---

## Frameworks

### 1. The IntOGen Driver Discovery Pipeline
A multi-method pipeline for identifying cancer driver genes from cohorts of tumor somatic mutations.

**Stage 1 — Input**: Somatic mutation calls from tumor cohorts (whole-exome or whole-genome sequencing).
**Stage 2 — Background modeling**: Estimate the expected neutral mutation rate per gene, accounting for trinucleotide context, gene length, and expression.
**Stage 3 — Signal detection (parallel methods)**:
  - OncodriveFM: detects bias toward high-functional-impact mutations
  - OncodriveCLUSTL: detects abnormal positional clustering of mutations
  - Oncodrive3D: detects clustering in 3D protein structure (using AlphaFold models)
  - dNdScv: detects elevated nonsynonymous-to-synonymous mutation ratio
**Stage 4 — Integration**: Combine p-values across methods; genes significant in multiple methods are high-confidence drivers.
**Stage 5 — Annotation**: Classify driver genes by role (oncogene vs. tumor suppressor via OncodriveROLE), tissue specificity, and mechanism.
**Output**: A compendium of cancer driver genes with evidence scores, available at intogen.org.

**Key insight**: No single signal is sufficient. The pipeline's power comes from combining orthogonal signals that capture different mechanisms of positive selection.

### 2. BoostDM — In Silico Saturation Mutagenesis
A framework for predicting the driver potential of every possible mutation in every cancer gene.

**Conceptual foundation**: Thousands of tumors have collectively tested the oncogenic potential of millions of mutations. These natural experiments can train machine learning models that generalize to untested mutations.
**Implementation**:
  - For each cancer gene × tissue combination, train a gradient boosting model on observed somatic mutations
  - Features: functional impact scores, evolutionary conservation, mutation clustering, structural context
  - Output: a probability score (0–1) for each possible mutation being a driver in that gene/tissue context
**Validation**: BoostDM models outperform experimental saturation mutagenesis in identifying driver vs. passenger mutations.
**Clinical application**: Integrated into CGI to interpret variants of uncertain significance in patient tumors.
**Scale**: 185 gene-tissue-specific models covering the most recurrent cancer driver genes.

### 3. Cancer Genome Interpreter (CGI) — Clinical Mutation Annotation
A tool for translating tumor somatic mutations into clinically actionable information.

**Input**: Somatic mutations from a patient's tumor (VCF or MAF format).
**Processing pipeline**:
  1. Identify driver mutations using IntOGen compendium and BoostDM models
  2. Annotate biomarkers of drug response (from curated databases of clinical evidence)
  3. Classify mutations by clinical actionability tier
**Output**: A structured report distinguishing driver from passenger mutations, identifying therapeutic targets, and flagging biomarkers for approved or investigational therapies.
**Design principle**: Interpretable, not a black box — every classification is traceable to evidence.
**Use case**: Supports oncologists in selecting targeted therapies for individual patients.

### 4. Mutational Landscape Decomposition — From Signatures to Mechanisms
A framework for understanding the mutagenic processes that shaped a tumor's genome.

**Observation**: The pattern of somatic mutations (trinucleotide context, strand bias, genomic distribution) reflects the mutational processes that generated them — UV exposure, tobacco carcinogens, APOBEC activity, defective DNA repair.
**Method**:
  1. Decompose the mutation spectrum into known COSMIC signatures
  2. Map signature activity to chromatin features (replication timing, nucleosome positioning, transcription factor binding)
  3. Identify how DNA repair deficiencies alter the mutation landscape
**Key finding**: Nucleotide excision repair (NER) is impaired at transcription factor binding sites and nucleosome-embedded DNA, creating local mutation hotspots. Somatic mutation rates exhibit a 10-bp periodicity tracking the DNA minor groove orientation around nucleosomes.
**Application**: Mutational footprints of chemotherapy agents can be identified in tumor genomes, enabling assessment of treatment-induced mutation burden.

### 5. Clonal Hematopoiesis Driver Discovery — Repurposing Cancer Genomics Methods
Applying cancer driver detection methods to identify genes driving clonal expansion in normal blood tissue.

**Problem**: Clonal hematopoiesis (CH) — the expansion of hematopoietic stem cell clones carrying somatic mutations — is a risk factor for hematologic malignancies and cardiovascular disease. The full compendium of CH driver genes is unknown.
**Approach**: "Reverse calling" — use tumor samples as reference to identify blood somatic mutations in 12,000+ cancer patients, then apply IntOGen to detect positive selection signals.
**Result**: ~70 CH driver genes identified, available at intogen.org/ch.
**Principle**: Methods developed for cancer are transferable to any clonal expansion process governed by positive selection.

---

## Mental Models

### The Needle-in-a-Haystack Problem
Of the thousands of mutations in a tumor, only 2–4 are drivers. Finding them requires not just looking harder, but looking smarter — using the right statistical framework (positive selection), the right scale (thousands of tumors), and the right combination of signals. The haystack is not random; it has structure (chromatin, replication timing, sequence context) that must be modeled to find the needle.

### Tumors as Replicated Natural Experiments
Each patient's tumor is an independent experiment testing the oncogenic potential of its mutations. Across thousands of patients, the same driver mutations recur because they confer the same selective advantage. This replication is the statistical foundation of driver detection: what is selected for will appear more often than chance predicts.

### The Mutation Rate Landscape as Terrain
The genome is not a flat surface for mutation accumulation. It is a terrain shaped by chromatin organization, replication timing, transcription factor binding, and nucleosome positioning. Some regions are mutation deserts (early-replicating, open chromatin, actively repaired); others are mutation mountains (late-replicating, heterochromatic, poorly repaired). Understanding this terrain is prerequisite to identifying the peaks that represent true driver hotspots rather than high-mutation-rate artifacts.

### The VUS Interpretation Bottleneck
Tumor sequencing generates thousands of variants; most are of uncertain significance. The bottleneck in precision oncology is not sequencing — it is interpretation. Every tool López-Bigas builds (IntOGen, BoostDM, CGI) is designed to attack this bottleneck: converting VUS into actionable classifications that guide treatment decisions.

### Cancer as a Continuous Darwinian Process
Cancer does not happen in a day. It is a gradual process of variation (random mutation) and selection (proliferative advantage) operating over years or decades. By the time a tumor is diagnosed, the cells have a long evolutionary history. This temporal dimension means that early-stage clonal expansions in healthy tissue (clonal hematopoiesis, field cancerization) are part of the same continuum — and understanding them is key to prevention.

### The Data-Interpretation Flywheel
"It's like a fish that eats its tail: the more data we have, the more information we can extract that helps us better interpret the next patient." Each new tumor genome adds to the training data for models, improves background estimates, and refines driver classifications. The system is self-improving: more data → better models → better interpretation → more clinical value → more sequencing → more data.

---

## Heuristics

1. **Always model the background before calling drivers** — a gene with many mutations in a high-mutation-rate region is not necessarily a driver; compare to the expected rate given chromatin context and trinucleotide composition.

2. **Combine orthogonal signals** — if two independent methods (e.g., clustering + functional impact bias) both flag a gene, confidence is multiplicatively higher than either alone.

3. **Use cohort size as a quality filter** — driver detection is unreliable in cohorts smaller than ~100 tumors; below this threshold, false discovery rates are unacceptably high.

4. **Distinguish gene-level from mutation-level drivers** — knowing that TP53 is a driver gene does not tell you which specific TP53 mutations are drivers; BoostDM addresses the second question, which is what matters clinically.

5. **Annotate by tissue type** — a mutation that drives lung cancer may be a passenger in colon cancer; driver status is gene × tissue specific, not universal.

6. **Treat the non-coding genome as a frontier, not a wasteland** — apply the same positive selection logic to promoters, UTRs, and lncRNAs; the methods work, the data is just harder to interpret.

7. **Validate computationally predicted drivers with orthogonal evidence** — functional experiments, structural data, and clinical outcomes all provide independent validation of computational predictions.

8. **Build tools that clinicians can use** — a driver prediction that requires a bioinformatician to interpret is not yet a clinical tool; the interface and output format matter as much as the algorithm.

9. **Make data and tools open** — the compendium of cancer drivers is a community resource; restricting access slows the entire field.

10. **Track mutational footprints of treatments** — chemotherapy leaves a mutational signature in tumor genomes; quantifying this signature enables assessment of treatment-induced mutation burden and secondary cancer risk.

---

## Anti-Patterns

### Recurrence-Only Driver Detection
Using mutation frequency as the sole criterion for driver identification misses low-frequency drivers (which may be highly tissue-specific or functionally potent) and generates false positives in genes with high background mutation rates. Recurrence is one signal among many, not a sufficient criterion.

### Ignoring the Background Mutation Rate
Calling a gene a driver because it has many mutations, without accounting for the local mutation rate (shaped by chromatin, replication timing, sequence context), is a fundamental error. Regions of high background mutation rate will produce false positives; regions of low background rate will produce false negatives.

### Treating All Mutations in a Driver Gene as Drivers
Once a gene is identified as a cancer driver, there is a temptation to treat all mutations in that gene as clinically significant. This is wrong: most mutations in driver genes are passengers. The distinction between driver and passenger mutations within a driver gene is the clinical question that BoostDM was built to answer.

### Black-Box Clinical Models
Machine learning models that produce driver predictions without interpretable features are inappropriate for clinical use. Oncologists need to understand why a mutation is classified as a driver to trust the classification and act on it. Interpretability is not a nice-to-have; it is a clinical requirement.

### Siloed Single-Cancer-Type Analysis
Analyzing one cancer type in isolation misses the opportunity to identify pan-cancer drivers and to use cross-cancer signal to improve statistical power. The IntOGen pipeline is designed to analyze all cancer types simultaneously, enabling both pan-cancer and tissue-specific driver identification.

### Neglecting Clonal Dynamics in Normal Tissue
Focusing exclusively on tumor genomes misses the pre-malignant phase of cancer development. Healthy tissue harbors clonal expansions driven by the same positive selection logic as tumors. Understanding these early clonal dynamics is essential for cancer prevention and early detection.

---

## Quotes

> "We start off with the idea that tumours follow a process of Darwinian evolution."
— IRB Barcelona "Meet Our Scientists" video, 2017

> "Of the thousands of mutations that we can find, perhaps only two, three or four are critical to transform a normal cell into a tumoural cell."
— IRB Barcelona "Meet Our Scientists" video, 2017

> "We look for what is referred to in evolution as positive selection."
— IRB Barcelona "Meet Our Scientists" video, 2017

> "I started slowly, and focused only on computational biology, no wet lab, and this really helped me make progress."
— ISCB Innovator Award profile, Bioinformatics, 2022

> "It was clear there were lots of mutations in tumors, and we thought it was important to understand how these mutations appear and which ones cause cancer across cancer types."
— ISCB Innovator Award profile, Bioinformatics, 2022

> "It's like a fish that eats its tail: the more data we have, the more information we can extract that helps us better interpret the next patient."
— El País interview, July 2023

> "Healthy tissue also has mutations that lead to cancer."
— El País interview, July 2023

> "Science is global and we have to make sure that ours is meaningful."
— IRB Barcelona "Meet Our Scientists" video, 2017

> "We want to develop methods to facilitate the medical interpretation of mutations and to help oncologists choose the most suitable treatment for each patient. This is how we contribute to furthering personalised medicine for cancer."
— IRB Barcelona "Meet Our Scientists" video, 2017

> "I was surprised to be selected and humbled and happy. It means the bioinformatics community appreciates and recognizes the work of my group."
— On receiving the 2022 ISCB Innovator Award

---

## Sources

- Martínez-Jiménez et al. (2020). "A compendium of mutational cancer driver genes." *Nature Reviews Cancer*. https://doi.org/10.1038/s41568-020-0290-x
- Muiños et al. (2021). "In silico saturation mutagenesis of cancer genes." *Nature*, 596, 428–432. https://doi.org/10.1038/s41586-021-03771-1
- González-Pérez & López-Bigas (2012). "Functional impact bias reveals cancer drivers." *Nucleic Acids Research*. https://doi.org/10.1093/nar/gks743
- Tamborero, González-Pérez & López-Bigas (2013). "OncodriveCLUST: exploiting the positional clustering of somatic mutations to identify cancer genes." *Bioinformatics*. https://doi.org/10.1093/bioinformatics/btt395
- Mularoni et al. (2016). "OncodriveFML: a general framework to identify coding and non-coding regions with cancer driver mutations." *Genome Biology*. https://doi.org/10.1186/s13059-016-0994-0
- Sabarinathan et al. (2016). "Nucleotide excision repair is impaired by binding of transcription factors to DNA." *Nature*. https://doi.org/10.1038/nature17661
- Pich et al. (2018). "Somatic and Germline Mutation Periodicity Follow the Orientation of the DNA Minor Groove around Nucleosomes." *Cell*. https://doi.org/10.1016/j.cell.2018.10.004
- Pich et al. (2019). "The mutational footprints of cancer therapies." *Nature Genetics*. https://doi.org/10.1038/s41588-019-0525-5
- González-Pérez, Sabarinathan & López-Bigas (2019). "Local Determinants of the Mutational Landscape of the Human Genome." *Cell*. https://doi.org/10.1016/j.cell.2019.02.051
- Fogg, Kovats & Vingron (2022). "2022 ISCB Innovator Award: Núria López-Bigas." *Bioinformatics*, 38(Suppl 1):i5–i6. https://pmc.ncbi.nlm.nih.gov/articles/PMC9235513/
- López-Bigas, N. (2023). Cambridge CRUK CI Seminar: "Tumor genomes shed light into somatic mutational processes and cancer vulnerabilities." https://talks.cam.ac.uk/talk/index/193834/
- Mouzo, J. (2023). "Núria López-Bigas, biologist: 'Healthy tissue also has mutations that lead to cancer'." *El País*. https://english.elpais.com/science-tech/2023-07-30/nuria-lopez-bigas-biologist-healthy-tissue-also-has-mutations-that-lead-to-cancer.html
