# Heuristics — Gad Getz

## Practical Rules for Cancer Genome Analysis

1. **Always use matched normals**: Somatic mutation calling without matched normal tissue leads to high false positive rates.

2. **Model the background mutation rate**: Genes with high mutation rates due to sequence context or replication timing will appear significant without proper background modeling.

3. **Use pan-cancer analysis for rare drivers**: Individual cancer types are too small to identify rare drivers; pan-cancer analysis is more powerful.

4. **Validate computationally identified drivers functionally**: Not all significantly mutated genes are drivers; functional validation is essential.

5. **Use standardized pipelines**: Reproducibility requires standardized, well-documented pipelines. Terra/FireCloud enables this.

6. **Consider tumor heterogeneity**: Bulk sequencing averages over clones; subclonal mutations may be missed.
