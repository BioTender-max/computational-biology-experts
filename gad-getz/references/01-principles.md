# Core Principles — Gad Getz

## 1. Background Mutation Rate is the Key
To find driver mutations, you must first model the background rate of passenger mutations. MutSig's power comes from its sophisticated background model.

## 2. Tumor-Normal Pairing is Essential
Somatic mutations can only be reliably identified by comparing tumor to matched normal tissue. MuTect's paired design is fundamental to its accuracy.

## 3. Pan-Cancer Analysis Reveals Universal Drivers
Analyzing many cancer types together reveals genes and pathways that are recurrently mutated across cancers — these are the most fundamental drivers.

## 4. Clonal Evolution Shapes the Tumor
Tumors consist of clones with different mutation profiles. Understanding clonal evolution is essential for understanding resistance and metastasis.

## 5. Reproducibility Requires Platforms
Large-scale cancer genomics requires standardized, reproducible pipelines. Terra/FireCloud enables the community to reproduce and extend TCGA analyses.
