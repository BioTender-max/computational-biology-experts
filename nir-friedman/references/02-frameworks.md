# Nir Friedman — Analytical Frameworks

## Bayesian Network Learning Framework
1. Discretize continuous expression data (or use continuous BN)
2. Choose scoring function (BDe for discrete, BIC for continuous)
3. Search structure space (greedy hill-climbing + random restarts)
4. Bootstrap to assess edge confidence
5. Validate high-confidence edges against known biology

## Module Network Framework
1. Initialize gene-to-module assignments randomly
2. E-step: For each module, find best regulator given current assignments
3. M-step: For each gene, find best module given current regulators
4. Repeat until convergence
5. Validate modules against known co-regulated gene sets

## cfChIP-seq Analysis Framework
1. Immunoprecipitate cell-free nucleosomes (H3K4me3, H3K27ac)
2. Sequence and align to reference genome
3. Call peaks (active promoters/enhancers)
4. Deconvolve tissue-of-origin using reference epigenomes (NNLS)
5. Identify differentially active regulatory elements between conditions
6. Infer gene expression programs from H3K4me3 profiles

## Chromatin State Analysis Framework
1. Profile multiple histone modifications simultaneously (ChIP-seq)
2. Learn combinatorial chromatin states (ChromHMM, Segway)
3. Assign functional annotations to states (active promoter, enhancer, repressed)
4. Track state transitions across conditions (differentiation, disease)
5. Identify regulatory elements driving state transitions
