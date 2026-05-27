# Anti-Patterns — Anshul Kundaje

## What to Avoid in Deep Learning for Regulatory Genomics

### Peak-Level Models
Coarse-grained models that operate on peaks rather than base pairs miss the combinatorial logic of TF binding. Base-pair resolution is essential.

### Black-Box Models Without Interpretation
Deep learning models must be interpreted to yield biological insight. Always use TF-MoDISco or similar tools.

### Ignoring Data Quality
ENCODE pipelines exist because data quality varies enormously. Uniform processing is essential for reproducibility.

### Overfitting to Training Cell Types
Models must be validated on held-out cell types and species. Overfitting to training data leads to poor generalization.

### Ignoring Sequence Context for Variants
Variant effects depend on the surrounding sequence context. Always score variants in their full genomic context.
