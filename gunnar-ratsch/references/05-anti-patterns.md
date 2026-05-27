# Anti-Patterns — Gunnar Rätsch

## What to Avoid in ML for Biomedicine

### Black-Box Models in Clinical Settings
Models that cannot explain their predictions are not trusted by clinicians. Always prioritize interpretability for clinical applications.

### Ignoring Spatial Context in Pathology
H&E images contain spatial information that coarse-grained models miss. Always use spatially-aware architectures.

### Overfitting to Training Cohorts
Clinical ML models must be validated on independent cohorts from different institutions. Single-cohort validation is insufficient.

### Disconnection from Clinical Practice
Computational methods developed without clinical input often fail to address real clinical problems. Always collaborate with clinicians.

### Ignoring Data Heterogeneity
Clinical data is heterogeneous — different institutions use different protocols, instruments, and coding systems. Always account for this heterogeneity.
