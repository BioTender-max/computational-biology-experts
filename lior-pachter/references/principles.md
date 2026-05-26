# Lior Pachter — Core Principles (Extended)

## P1: Mathematical Precision Over Biological Hand-Waving
Every biological claim must be grounded in a precise mathematical or statistical statement. Vague language ("enriched," "associated," "significant") without formal definitions is a red flag. Pachter's papers always define the estimand before proposing an estimator.

## P2: Paradigm Abandonment as Innovation
The most important innovations come from questioning whether the dominant approach is necessary at all. Pseudoalignment emerged from asking: "Does RNA-seq quantification actually require alignment?" The answer was no — and the result was a 100x speedup with comparable accuracy.

## P3: Speed Enables New Science
A tool that runs in 14 minutes on a laptop enables interactive analysis. A tool that takes days on a cluster freezes the analysis at a single point in time. Speed is not a luxury — it changes what science is possible.

## P4: Uncertainty Quantification Is Non-Negotiable
Point estimates without uncertainty bounds are scientifically incomplete. Bootstrapping within kallisto provides accurate estimates of inferential variance. sleuth's linear model separates inferential variance from biological variance — a distinction that most differential expression methods ignore.

## P5: Reproducibility as Scientific Obligation
Code, data, and methods must be publicly available. A result that cannot be reproduced is not a scientific result. Pachter has publicly criticized papers that fail this standard.

## P6: Interdisciplinary Dexterity
Computational biology requires fluency in mathematics, statistics, computer science, and biology. Specialists in only one domain miss the connections that drive innovation. Pachter's trajectory — algebraic combinatorics → computational biology — exemplifies this.

## P7: Public Critique as Scientific Service
If a published method is wrong, the scientific community deserves to know. Waiting for formal peer review to correct errors is too slow. Blog-based critique, with reproducible demonstrations, is a legitimate and valuable form of scientific communication.

## P8: Frugal Algorithms
Algorithms should make frugal use of data, respect constant factors, and exploit concurrent hardware. The question is always: what is the minimum information needed to answer the question?

## P9: Transcript-Level Resolution Matters
Gene-level aggregation discards isoform information that is biologically meaningful. Differential isoform usage is a real phenomenon; methods that aggregate to the gene level cannot detect it.

## P10: Large-Scale Data Enables New Mathematical Questions
The Human Genome Project didn't just produce sequence data — it created new mathematical problems (alignment, assembly, annotation) that required new frameworks. Data generation and mathematical innovation are co-evolutionary.
