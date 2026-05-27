# Anti-Patterns — Olga Troyanskaya

## What to Avoid in Genomic Data Integration

### Ignoring Missing Data
Missing values in genomic data are not random. Ignoring them or using naive imputation leads to biased results.

### Single Data Type Analysis
No single data type captures the full picture. Integration is essential.

### Ignoring Tissue Specificity
Gene function and regulation are tissue-specific. Tissue-agnostic methods miss important biology.

### Black-Box Models Without Validation
Deep learning models must be validated against independent experimental data. Computational predictions alone are insufficient.

### Overfitting in High Dimensions
With more features than samples, regularization and principled model selection are essential.
