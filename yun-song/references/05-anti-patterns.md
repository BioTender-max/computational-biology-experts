# Anti-Patterns — Yun Song

## What to Avoid in Probabilistic Computational Biology

### Ignoring Model Assumptions
Statistical models make assumptions; violating them leads to incorrect inference. Always check whether your data satisfies the model assumptions.

### Computational Inefficiency
Algorithms that don't scale to genome-wide data are impractical. Always consider computational complexity.

### Ignoring Uncertainty
Point estimates without uncertainty quantification mislead users. Always report credible intervals.

### Overfitting
With large genomic datasets, overfitting is a constant risk. Use regularization and cross-validation.

### Ignoring Recombination
Recombination breaks up haplotypes and violates the assumptions of many population genetics models. Always account for recombination.
