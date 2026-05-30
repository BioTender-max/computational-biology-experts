# Anti-Patterns — Núria López-Bigas

## 1. Recurrence-Only Driver Detection

**The mistake**: Using mutation frequency as the sole criterion for driver identification.

**Why it fails**: Misses low-frequency drivers (which may be highly tissue-specific or functionally potent) and generates false positives in genes with high background mutation rates (large genes, genes in late-replicating regions). Recurrence is one signal among many, not a sufficient criterion.

**The fix**: Combine recurrence with functional impact bias, positional clustering, and 3D structural clustering. Use the IntOGen multi-method approach.

---

## 2. Ignoring the Background Mutation Rate

**The mistake**: Calling a gene a driver because it has many mutations, without accounting for the local mutation rate shaped by chromatin, replication timing, and sequence context.

**Why it fails**: Regions of high background mutation rate will produce false positives (genes that appear mutated above expectation only because the expectation was underestimated). Regions of low background rate will produce false negatives (drivers missed because the signal is diluted by a poorly estimated background).

**The fix**: Use trinucleotide context normalization, account for replication timing and chromatin accessibility, and validate background estimates against synonymous mutations (assumed neutral).

---

## 3. Treating All Mutations in a Driver Gene as Drivers

**The mistake**: Once a gene is identified as a cancer driver, treating all mutations in that gene as clinically significant.

**Why it fails**: Most mutations in driver genes are passengers. A TP53 missense mutation at a hotspot residue is a driver; a TP53 missense mutation at a non-conserved residue may be a passenger. The distinction between driver and passenger mutations within a driver gene is the clinical question that BoostDM was built to answer.

**The fix**: Apply mutation-level driver scoring (BoostDM) to every mutation in a driver gene, not just gene-level driver classification.

---

## 4. Black-Box Clinical Models

**The mistake**: Deploying machine learning models for clinical mutation interpretation that produce predictions without interpretable features.

**Why it fails**: Oncologists need to understand why a mutation is classified as a driver to trust the classification and act on it. A black-box model that says "this mutation is a driver with 87% probability" without explaining which features drove that prediction is not clinically useful and may be dangerous.

**The fix**: Design models with interpretable features from the start. Use gradient boosting with SHAP values, or other methods that allow feature attribution. Ensure every classification is traceable to specific biological evidence.

---

## 5. Siloed Single-Cancer-Type Analysis

**The mistake**: Analyzing one cancer type in isolation, without leveraging cross-cancer signal.

**Why it fails**: Misses the opportunity to identify pan-cancer drivers and to use cross-cancer signal to improve statistical power for rare cancer types. Many driver genes are shared across cancer types; analyzing them together increases the number of mutations available for training and validation.

**The fix**: Design pipelines that analyze all cancer types simultaneously, enabling both pan-cancer and tissue-specific driver identification. Use the IntOGen approach of running the pipeline across 66+ cancer types.

---

## 6. Neglecting Clonal Dynamics in Normal Tissue

**The mistake**: Focusing exclusively on tumor genomes and ignoring the pre-malignant phase of cancer development.

**Why it fails**: Healthy tissue harbors clonal expansions driven by the same positive selection logic as tumors. Understanding these early clonal dynamics is essential for cancer prevention and early detection. A cancer genomics program that only studies tumors is studying the end stage of a process that began years or decades earlier.

**The fix**: Design studies that sequence matched normal tissue alongside tumors. Apply cancer driver detection methods to clonal hematopoiesis and other pre-malignant conditions. Develop methods for detecting clonal expansions in normal tissue using deep sequencing.
