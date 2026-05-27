# Alkes Price — Anti-Patterns

## Anti-Pattern 1 — Ignoring population stratification
Failing to correct for ancestry leads to spurious associations. Always include principal components as covariates and check the LDSC intercept.

## Anti-Pattern 2 — Confusing polygenicity with confounding
Inflated GWAS statistics can be caused by either polygenicity or confounding. Use LDSC to distinguish these — the intercept estimates confounding, the slope estimates heritability.

## Anti-Pattern 3 — Reporting only GWAS hits, not heritability
GWAS hits explain only a fraction of heritability. Always report SNP heritability to give context for the hits.

## Anti-Pattern 4 — Using the wrong reference panel for LD estimation
LD patterns differ across populations. Using a European reference panel for a non-European GWAS leads to biased LDSC estimates. Use an ancestry-matched reference panel.

## Anti-Pattern 5 — Ignoring sample overlap in genetic correlation analysis
If two GWAS share samples, the genetic correlation estimate is inflated. Use the LDSC intercept to detect and correct for sample overlap.

## Anti-Pattern 6 — Over-interpreting functional enrichment
A functional category that is enriched for heritability is not necessarily causal — it may be in LD with the true causal category. Use conditional analysis to distinguish enrichment from LD.

## Anti-Pattern 7 — Using small samples for heritability estimation
LDSC requires large sample sizes (N > 5,000) for reliable heritability estimates. With small samples, the estimates are noisy and potentially biased.
