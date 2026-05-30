# IntOGen — Cancer Driver Gene Compendium

IntOGen (Integrative OncoGenomics) is a pipeline and database for
identifying cancer driver genes across tumor types. The 2020 compendium
identified 568 cancer driver genes across 66 cancer types from >28,000
tumor samples using 6 complementary statistical methods.

**Key features:**
- 6 driver discovery methods (OncodriveFML, dNdScv, MutPanning, etc.)
- 66 cancer types, >28,000 tumors
- Ranked driver gene lists per cancer type
- Freely available at intogen.org

**Reference:** Martínez-Jiménez et al., Nature Reviews Cancer (2020). PMID: 32778778

---

# BoostDM — Driver Mutation Identification

BoostDM is a machine learning model that predicts whether a specific
somatic mutation in a specific gene and tissue is a cancer driver.
Trained on tumor somatic mutations, it enables in silico saturation
mutagenesis — computationally testing every possible mutation in a
cancer gene.

**Key features:**
- Tissue-specific driver mutation prediction
- In silico saturation mutagenesis
- Trained on >28,000 tumor samples
- Interpretable feature importance

**Reference:** Muiños et al., Nature Methods (2021). PMID: 34385711