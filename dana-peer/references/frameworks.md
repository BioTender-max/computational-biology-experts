# Dana Pe'er — Conceptual Frameworks

## Framework 1: Single-Cell Trajectory Analysis
**Problem**: Cells exist along a continuum of developmental states, but traditional methods discretize them into clusters.

**Wanderlust** (2014):
- Input: single-cell mass cytometry or RNA-seq data
- Method: graph-based algorithm; aligns cells onto a 1D developmental trajectory
- Output: pseudotime ordering of cells along a developmental continuum
- Application: human B cell lymphopoiesis; revealed nascent fractions of B cell progenitors

**Palantir** (2019):
- Input: single-cell RNA-seq data
- Method: Markov chain model of differentiation; treats cell fate as a probabilistic process
- Output: pseudotime ordering + probability of reaching each terminal state + entropy (plasticity measure)
- Application: human bone marrow hematopoiesis; identification of key TFs driving lineage fate choice

**Key insight**: Differentiation is not deterministic — cells have probabilities of reaching different terminal states. Entropy measures how much plasticity a cell retains.

---

## Framework 2: Cellular Plasticity and Cancer
**Core insight**: Cancer cells don't create new gene programs — they access gene programs that normally exist for other biological purposes (development, regeneration).

**"Mix-and-match buffet"**: Metastatic cells combine gene programs across many different cell types, endowing them with new abilities to adapt to different environments.

**Epigenetic plasticity**: Not genetic mutations but the ability to access gene programs that normally are associated with other cell types — including early developmental and embryonic programs that should not be accessed by adult cells.

**Application**: Pancreatic tumorigenesis (Science 2023); small cell lung cancer; prostate cancer regeneration.

---

## Framework 3: Data Diffusion for Single-Cell Imputation (MAGIC)
**Problem**: Single-cell RNA-seq data is extremely sparse — most genes are not detected in most cells (dropout).

**Solution**: MAGIC (Markov Affinity-based Graph Imputation of Cells):
1. Build a cell-cell similarity graph (k-nearest neighbors)
2. Compute a Markov transition matrix (diffusion operator)
3. Apply diffusion to impute missing values
4. Recover gene-gene relationships from imputed data

**Key insight**: The manifold structure of single-cell data can be exploited to impute missing values without introducing artifacts.

---

## Framework 4: Supervised Gene Program Discovery (Spectra)
**Problem**: Single-cell data contains many overlapping gene programs; unsupervised methods (NMF, PCA) don't leverage prior biological knowledge.

**Solution**: Spectra — supervised discovery of interpretable gene programs from single-cell data. Incorporates prior knowledge (gene sets, pathways) as constraints.

**Output**: Interpretable gene programs that correspond to known biological processes, plus novel programs not captured by prior knowledge.
