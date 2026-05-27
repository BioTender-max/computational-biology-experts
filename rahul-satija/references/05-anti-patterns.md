# Rahul Satija — Anti-Patterns

## Batch Effect Blindspot
Running clustering without batch correction when samples come from different experiments produces clusters reflecting technical variation, not biology.

## Log-Normalization Default
Log-normalization is suboptimal for datasets with variable sequencing depth. SCTransform is more principled.

## Single-Modality Limitation
Analyzing RNA and protein separately in CITE-seq data misses complementary information. Use WNN.

## Resolution Sensitivity
Clustering resolution dramatically affects the number of clusters. Always test multiple resolutions.

## UMAP Distance Fallacy
Distances between clusters in UMAP space are not biologically meaningful.
