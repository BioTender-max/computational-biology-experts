# Nir Friedman — Anti-Patterns to Avoid

## The Undirected Network Mistake
Reporting an undirected network as if it were a Bayesian network conflates two different mathematical objects. Undirected edges cannot be interpreted as regulatory relationships without additional assumptions.

## The Discretization Artifact
Discretizing continuous expression data into bins introduces artifacts that depend on the choice of bin boundaries. Results should be robust to different discretization schemes.

## The Multiple Testing Blindspot
When learning networks over thousands of genes, the number of possible edges is O(n²). Without correction for multiple testing, many spurious edges will appear significant.

## The cfDNA Contamination Problem
Cell-free DNA is contaminated with genomic DNA from lysed cells during blood processing. Careful sample handling and computational contamination detection are essential.

## The Reference Epigenome Mismatch
Tissue deconvolution of cfChIP-seq requires reference epigenomes that match the contributing cell types. Using wrong reference epigenomes gives incorrect deconvolution results.

## The Temporal Confounding Error
In time-series gene expression data, apparent regulatory relationships may reflect temporal autocorrelation rather than true regulation. Always include time as a covariate.

## The Single-Dataset Conclusion
Conclusions from a single dataset may not generalize. Always validate in independent datasets from different labs, protocols, and species.
