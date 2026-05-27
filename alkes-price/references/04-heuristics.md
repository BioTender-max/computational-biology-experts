# Alkes Price — Heuristics

1. Always correct for population stratification — include top PCs as covariates in GWAS.
2. Use LD score regression to assess confounding — check the LDSC intercept before interpreting results.
3. Report SNP heritability, not just GWAS hits — heritability tells you how much genetic signal there is.
4. Use stratified LDSC to identify enriched functional categories — it reveals the functional architecture.
5. Compute genetic correlations between related traits — they reveal shared biology.
6. Use summary statistics, not individual-level data, when possible — they enable large-scale meta-analysis.
7. Include functional annotation in fine-mapping — it improves causal variant identification.
8. Use the baseline model as a starting point for stratified LDSC — it captures known functional categories.
9. Check for sample overlap in genetic correlation analysis — it inflates the intercept.
10. Use large reference panels for LD estimation — 1000 Genomes or UK Biobank.
11. Report confidence intervals, not just point estimates — heritability estimates have uncertainty.
12. Be skeptical of heritability estimates from small samples — LDSC requires large N.
13. Use functionally-informed polygenic scores — they outperform standard PRS.
14. Consider ancestry-specific LD patterns — LD differs across populations.
15. Use cross-ancestry GWAS to improve fine-mapping — different LD patterns help localize causal variants.
16. Validate methods on simulations — always check that the method works when the truth is known.
17. Share summary statistics — they enable replication and meta-analysis.
18. Use the genomic inflation factor as a diagnostic — λ > 1.1 warrants investigation.
19. Consider the effective sample size — case-control imbalance reduces effective N.
20. Use multiple testing correction — genome-wide significance threshold is 5×10⁻⁸.
