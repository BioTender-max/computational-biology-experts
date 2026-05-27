# Alkes Price — Mental Models

## "The genomic inflation factor as a diagnostic"
The genomic inflation factor λ (median chi-squared / 0.456) measures overall inflation of GWAS test statistics. λ > 1 indicates either polygenicity or confounding. LD score regression distinguishes these: if inflation is proportional to LD scores, it's polygenicity; if uniform, it's confounding.

## "LD score as a measure of information"
A variant with a high LD score is in LD with many other variants — it "tags" a large region of the genome. Under a polygenic model, high-LD-score variants have higher expected chi-squared statistics because they tag more causal variants.

## "Heritability partitioning as a functional map"
Stratified LDSC produces a map of heritability across functional categories — which categories are enriched, which are depleted. For autoimmune diseases, regulatory elements in immune cells are enriched; for neurological traits, brain-specific regulatory elements are enriched.

## "Genetic correlation as a measure of shared biology"
Two traits with genetic correlation r_g = 0.8 share 80% of their genetic architecture. This has implications for drug repurposing, comorbidity, and biological mechanism.

## "Summary statistics as a public good"
GWAS summary statistics can be shared without sharing individual-level data, enabling large-scale meta-analysis and method development. Price has consistently advocated for sharing summary statistics.

## "The baseline model as a null hypothesis"
The stratified LDSC baseline model (53 functional categories) represents current understanding of functional genomics. A new functional category is informative if it explains heritability beyond what the baseline model captures.
