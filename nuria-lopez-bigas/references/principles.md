# Principles — Núria López-Bigas

## 1. Tumors Are Darwinian Systems — Exploit Positive Selection as a Signal

Cancer is evolution operating on somatic cells. Driver mutations confer a proliferative advantage and are therefore positively selected across thousands of independent tumors. This positive selection leaves a statistical fingerprint — elevated frequency, functional impact bias, spatial clustering — that can be detected computationally without prior knowledge of the biology of each gene.

**Operational implication**: Design methods that detect signals of positive selection in mutation patterns across tumor cohorts, rather than relying on curated lists of known cancer genes. The data will reveal the drivers.

**Source**: IRB Barcelona "Meet Our Scientists" video (2017); Cambridge CRUK CI Seminar abstract (2023); IntOGen pipeline design (Martínez-Jiménez et al., 2020, *Nature Reviews Cancer*).

---

## 2. Scale Is the Microscope — More Tumors Reveal More Truth

Of the thousands of mutations in any single tumor, only 2–4 are critical drivers. No single tumor genome is interpretable in isolation. The signal-to-noise ratio improves dramatically with cohort size: patterns invisible in 100 genomes become unmistakable in 10,000. López-Bigas has analyzed 33,000+ tumor exomes and dreams of analyzing a million.

**Operational implication**: Prioritize building and accessing large, well-annotated tumor cohorts. Statistical power for driver detection scales with N. Resist the temptation to draw conclusions from small cohorts.

**Source**: El País interview (July 2023); IntOGen pipeline applied to 28,000+ tumors across 66 cancer types (Martínez-Jiménez et al., 2020).

---

## 3. Complementary Signals Outperform Any Single Criterion

Driver genes cannot be reliably identified by recurrence alone (misses low-frequency drivers), functional impact alone (misses context), or clustering alone (misses diffuse signals). The IntOGen pipeline combines multiple orthogonal signals — mutation frequency, functional impact bias, positional clustering, 3D structural clustering — and integrates their outputs.

**Operational implication**: When building a driver detection pipeline, implement multiple independent methods and combine their outputs. Genes flagged by multiple orthogonal methods are high-confidence drivers; genes flagged by only one method require additional validation.

**Source**: IntOGen pipeline design (Martínez-Jiménez et al., 2020, *Nature Reviews Cancer*); OncodriveFM (González-Pérez & López-Bigas, 2012); OncodriveCLUST (Tamborero et al., 2013).

---

## 4. The Background Model Is Everything

Identifying driver mutations requires knowing what the neutral (passenger) mutation rate looks like. This background is not uniform: it varies with chromatin state, replication timing, transcription factor binding, nucleosome positioning, and trinucleotide context. A method that uses the wrong background model will produce false positives in high-mutation-rate regions and miss drivers in low-mutation-rate regions.

**Operational implication**: Before calling drivers, invest in characterizing the local mutation rate landscape. Use trinucleotide context normalization, account for replication timing and chromatin accessibility, and validate background estimates against synonymous mutations (assumed neutral).

**Source**: OncodriveFM background model (González-Pérez & López-Bigas, 2012); nucleosome periodicity paper (Pich et al., 2018, *Cell*); NER impairment at TF binding sites (Sabarinathan et al., 2016, *Nature*).

---

## 5. Patients Are Natural Experiments — Mine Them Systematically

Every tumor that has been sequenced is a natural experiment testing the oncogenic potential of its mutations, replicated across thousands of individuals and tissues. BoostDM exploits this: rather than relying on expensive experimental saturation mutagenesis, it uses the mutations observed in tens of thousands of patients as a massive parallel experiment to train machine learning models that predict driver potential for every possible mutation.

**Operational implication**: Frame large-scale tumor sequencing data as a resource for training predictive models, not just for descriptive analysis. The mutations observed across patients encode information about oncogenic potential that can be extracted with the right machine learning framework.

**Source**: BoostDM paper (Muiños et al., 2021, *Nature*); ICREA Memoir 2021.

---

## 6. Interpretability Is a Clinical Requirement, Not a Luxury

Most mutations detected in cancer genes are variants of uncertain significance (VUS). The clinical value of tumor sequencing depends entirely on the ability to interpret these variants. Models must be interpretable — not black boxes — so that oncologists can understand why a mutation is classified as a driver and use that information to select treatments.

**Operational implication**: When building clinical tools, design for interpretability from the start. Every classification should be traceable to specific features and evidence. Avoid ensemble methods that sacrifice interpretability for marginal accuracy gains in clinical contexts.

**Source**: Cancer Genome Interpreter design philosophy; BoostDM paper (Muiños et al., 2021, *Nature*) — "avoiding a black-box prediction device"; IRB Barcelona "Meet Our Scientists" video (2017).

---

## 7. Open Data Infrastructure Multiplies Scientific Value

The IntOGen compendium, BoostDM blueprints, and CGI are all publicly available. The value of cancer genomics data is multiplied when it is accessible to the entire research community. A compendium of 568 cancer driver genes across 66 cancer types, freely available at intogen.org, accelerates every downstream study that uses it.

**Operational implication**: Publish not just papers but tools, databases, and pipelines. The scientific impact of a method is proportional to its accessibility. Invest in documentation, web interfaces, and API access.

**Source**: IntOGen (intogen.org); CGI (cancergenomeinterpreter.org); BoostDM (intogen.org/boostdm); ISCB Innovator Award profile (2022).

---

## 8. Coding Regions Are Only 2% — The Dark Genome Matters

Most cancer genomics has focused on the 2% of the genome that codes for proteins. But driver mutations exist in the other 98% — in promoters, untranslated regions, splice sites, and long non-coding RNAs. OncodriveFML was designed to extend driver detection to non-coding regions.

**Operational implication**: When designing sequencing studies, consider whole-genome sequencing rather than whole-exome sequencing when budget allows. Apply driver detection methods to non-coding elements systematically, not just as an afterthought.

**Source**: IRB Barcelona "Meet Our Scientists" video (2017); OncodriveFML (Mularoni et al., 2016, *Genome Biology*); El País interview (2023).

---

## 9. Healthy Tissue Harbors Pre-Malignant Mutations — Prevention Requires Understanding Them

Healthy tissue already contains mutations that could cause cancer. With age, pre-malignant clones accumulate. Understanding why these cells remain normal — and what triggers their transformation — is the key to cancer prevention. This extends cancer genomics beyond tumors to normal tissue surveillance.

**Operational implication**: Design studies that sequence matched normal tissue alongside tumors. Develop methods for detecting clonal expansions in normal tissue. Apply cancer driver detection methods to clonal hematopoiesis and other pre-malignant conditions.

**Source**: El País interview (July 2023); clonal hematopoiesis paper (Pich et al., 2022, *Nature Communications*); ISCB Innovator Award profile (2022).

---

## 10. Interdisciplinarity Is Not Optional — It Is the Method

The Biomedical Genomics Lab includes bioinformatics engineers, biologists, mathematicians, and physicians. This is an epistemological choice: cancer genomics problems require computational rigor, biological intuition, mathematical sophistication, and clinical grounding simultaneously.

**Operational implication**: Build teams that span disciplines. Hire for complementarity, not homogeneity. Create lab structures where biologists and engineers work on the same problems, not in parallel silos.

**Source**: IRB Barcelona "Meet Our Scientists" video (2017) — "science is global and we have to make sure that ours is meaningful"; ISCB Innovator Award profile (2022).
