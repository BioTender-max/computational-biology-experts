# Anti-Patterns — Stein Aerts

## What to Avoid in Regulatory Genomics

### Ignoring Regulatory Heterogeneity
Bulk epigenomics misses cell-type-specific regulatory programs. Single-cell resolution is essential for understanding regulatory diversity.

### Treating Enhancers as Binary
Enhancer activity is quantitative and context-dependent. Binary (active/inactive) classifications miss important regulatory information.

### Overfitting Deep Learning Models
Models trained on one tissue or species may not generalize. Always validate on held-out cell types and species.

### Neglecting Experimental Validation
Computational predictions of enhancer activity must be tested with reporter assays. Computational predictions alone are insufficient.

### Ignoring TF Combinatorics
Enhancer activity is determined by combinations of TFs, not individual TFs. Models that ignore combinatorial logic miss important regulatory mechanisms.
