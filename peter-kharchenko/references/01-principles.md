# Peter Kharchenko — Core Principles

1. **Technical noise is the central challenge.** Dropout events, overdispersion, and batch effects must be modeled explicitly.
2. **The cellular detection rate is a major confounder.** Always include CDR as a covariate in statistical models.
3. **RNA velocity reveals cell state dynamics.** The ratio of unspliced to spliced mRNA encodes the direction of transcriptional change.
4. **Spatial context requires new statistical methods.** Spatial transcriptomics data has fundamentally different structure from dissociated single-cell data.
5. **Tumor heterogeneity requires single-cell resolution.** CNV inference from scRNA-seq enables identification of tumor cells without separate WGS.
6. **Bayesian methods provide principled uncertainty quantification.** Every prediction should come with a confidence interval.
7. **Multi-dataset integration requires careful statistical modeling.** Conos integrates multiple datasets without batch correction by building a joint graph.
