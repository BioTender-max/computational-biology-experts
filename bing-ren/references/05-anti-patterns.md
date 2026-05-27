# Bing Ren — Anti-Patterns

## Enhancer-Gene Assignment by Proximity
Assigning enhancers to target genes based on proximity alone is inaccurate. Use Hi-C or ABC model.

## Bulk Epigenomics Averaging
Bulk ChIP-seq averages over all cells. Use single-cell ATAC-seq to resolve cell-type-specific programs.

## Peak Calling Sensitivity-Specificity Tradeoff
Loose peak calling increases sensitivity but also false positives. Always validate key peaks.

## TAD Boundary Artifact
TAD boundaries from low-resolution Hi-C are noisy. Use sufficient sequencing depth.

## Compartment-TAD Confusion
A/B compartments and TADs are different features at different scales. Don't conflate them.
