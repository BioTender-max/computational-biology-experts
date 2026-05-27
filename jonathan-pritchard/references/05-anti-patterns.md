# Jonathan Pritchard — Anti-Patterns

## Anti-Pattern 1 — Ignoring population stratification
Failing to control for population structure in GWAS leads to spurious associations. Always include principal components or use a mixed model that accounts for relatedness and ancestry.

## Anti-Pattern 2 — Over-interpreting individual GWAS hits
A GWAS hit is a statistical association, not a mechanism. The causal variant may be in LD with the hit; the causal gene may be far from the hit; the mechanism may be regulatory, not coding.

## Anti-Pattern 3 — Assuming hard sweeps are the dominant mode of adaptation
Most recent human evolution is polygenic, not driven by hard sweeps. Single-locus selection tests (iHS, XP-EHH) have low power for polygenic adaptation. Use polygenic score comparisons instead.

## Anti-Pattern 4 — Choosing K in STRUCTURE by visual inspection
The number of ancestral populations K should be chosen by cross-validation or log-likelihood comparison, not by visual inspection of the bar plots. Visual inspection is subjective and biased.

## Anti-Pattern 5 — Treating GWAS hits as the complete genetic architecture
GWAS hits explain only a fraction of heritability. The omnigenic model predicts that thousands of additional variants contribute. Polygenic scores capture more of the architecture.

## Anti-Pattern 6 — Ignoring gene regulatory networks
Most GWAS hits act through gene regulation. Interpreting them without considering the regulatory context misses the biology.

## Anti-Pattern 7 — Failing to replicate
The history of human genetics is full of associations that failed to replicate. Always replicate in an independent cohort before claiming a discovery.
