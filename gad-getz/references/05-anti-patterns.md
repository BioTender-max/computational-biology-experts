# Anti-Patterns — Gad Getz

## What to Avoid in Cancer Genome Analysis

### Ignoring Background Mutation Rate
Genes with high mutation rates due to sequence context or replication timing will appear significant without proper background modeling. MutSig was designed to address this.

### Not Using Matched Normals
Somatic mutation calling without matched normal tissue leads to high false positive rates. Always use matched normals.

### Ignoring Tumor Heterogeneity
Bulk sequencing averages over clones; subclonal mutations may be missed. Consider clonal decomposition methods.

### Confusing Correlation with Causation
Not all significantly mutated genes are drivers; functional validation is essential.

### Using Non-Standardized Pipelines
Non-standardized pipelines lead to irreproducible results. Always use well-documented, standardized pipelines.
