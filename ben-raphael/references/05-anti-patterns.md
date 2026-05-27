# Anti-Patterns — Ben Raphael

## What to Avoid in Algorithmic Cancer Genomics

### Single-Sample Analysis of Heterogeneous Tumors
Single samples miss the clonal architecture. Multi-sample analysis is essential for understanding tumor evolution.

### Ignoring Allele Specificity
Copy-number analysis without allele resolution misses important evolutionary events, including whole-genome duplication.

### Confusing Driver and Passenger Mutations
Not all mutations are drivers; statistical methods are needed to distinguish them. Functional validation is essential.

### Ignoring Whole-Genome Duplication
WGD is common in cancer and profoundly affects copy-number interpretation. Always check for WGD before interpreting copy-number profiles.

### Using Heuristic Algorithms Without Validation
Heuristic algorithms may give wrong answers on real data. Always validate on simulated data with known ground truth.
