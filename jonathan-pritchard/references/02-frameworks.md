# Jonathan Pritchard — Conceptual Frameworks

## Framework 1 — The STRUCTURE Model
STRUCTURE models each individual as a mixture of K ancestral populations, each characterized by allele frequencies at each locus. Uses Bayesian inference (MCMC) to estimate admixture proportions. K chosen by cross-validation or log-likelihood plateau.

**Tools**: STRUCTURE, ADMIXTURE, fastSTRUCTURE

## Framework 2 — The Omnigenic Model
Complex traits are influenced by essentially all genes expressed in relevant tissues, because gene regulatory networks are highly interconnected. "Core genes" directly affect the trait; "peripheral genes" affect it indirectly through regulatory networks. Most GWAS hits are peripheral genes.

**Implications**: Heritability is spread across the entire genome; functional annotation requires understanding gene regulatory networks.

## Framework 3 — Polygenic Adaptation
Natural selection shifts the mean of a quantitative trait by changing allele frequencies at many loci simultaneously. Each locus shows only a tiny frequency change — invisible to single-locus tests — but detectable by comparing polygenic scores across populations.

**Detection**: Qst-Fst comparison; Turchin et al. method; Racimo et al. method

## Framework 4 — LD Score Regression for Heritability
Uses the relationship between GWAS chi-squared statistics and LD scores to estimate SNP heritability and genetic correlation. Robust to population stratification.

**Tools**: LDSC software (ldsc.py)

## Framework 5 — eQTL Integration
Expression QTLs (eQTLs) are genetic variants affecting gene expression. Integrating eQTL data with GWAS identifies causal genes and tissues.

**Tools**: GTEx, coloc, TWAS/PrediXcan, Mendelian randomization
