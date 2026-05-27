# Fabian Theis — Heuristics & Rules of Thumb

1. **Filter cells with >20% mitochondrial reads.** They're dying. Filter genes expressed in <3 cells — they're noise. But always look at the distributions before choosing thresholds.

2. **Use 50 PCs for standard analysis.** More PCs add noise; fewer lose signal. For trajectory analysis, use more PCs (100) to preserve fine structure.

3. **Check for batch effects before analysis.** If your UMAP clusters by batch before clustering by biology, you have a batch effect problem. scVI or Harmony will fix it.

4. **Validate RNA velocity directions against known biology.** RNA velocity is most reliable for fast, transient processes. For slow processes, the signal is weak. Always validate against known biology.

5. **Use Leiden clustering, not k-means.** Leiden is more principled for graph-based clustering and produces more biologically meaningful clusters.

6. **Automated annotation is a starting point.** Always validate automated annotations with marker gene expression and, when possible, orthogonal methods.

7. **Use negative binomial likelihood for count data.** scRNA-seq counts are overdispersed. Negative binomial (or zero-inflated NB) is more appropriate than Poisson or Gaussian.

8. **Validate batch correction by checking biological variation.** After batch correction, check that known biological differences (cell types, conditions) are still visible. Overcorrection removes real biology.
