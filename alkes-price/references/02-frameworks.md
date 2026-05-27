# Alkes Price — Conceptual Frameworks

## Framework 1 — PCA for Population Stratification Correction
PCA of the genotype matrix captures major axes of population variation. Including top PCs as covariates in GWAS regression removes confounding by ancestry. Number of PCs depends on degree of population structure.

**Tools**: PLINK, EIGENSOFT; include top 10–20 PCs as covariates

## Framework 2 — LD Score Regression
Exploits the relationship between GWAS chi-squared statistics and LD scores. Under a polygenic model, chi-squared statistics are proportional to LD scores; under confounding, they are uniformly inflated. Intercept estimates confounding; slope estimates heritability.

**Formula**: E[χ²_j] = Nh²/M × l_j + Na + 1
**Tools**: LDSC software (ldsc.py); --h2 for heritability, --rg for genetic correlation

## Framework 3 — Stratified LD Score Regression
Partitions heritability across functional categories by computing category-specific LD scores. Enrichment = fraction of heritability / fraction of variants.

**Tools**: LDSC with --ref-ld-chr pointing to category-specific LD scores; baseline model (53 functional categories)

## Framework 4 — Functionally-Informed Fine-Mapping
Incorporates functional annotation as a prior probability of causality to improve fine-mapping accuracy. PolyFun uses stratified LDSC to estimate prior probabilities.

**Tools**: SuSiE, FINEMAP, PolyFun

## Framework 5 — Polygenic Score Methods
Aggregate effects of many variants to predict individual-level phenotypes. Use LD information and functional annotation to improve prediction accuracy.

**Tools**: PRS-CS, LDpred2, SBayesR
