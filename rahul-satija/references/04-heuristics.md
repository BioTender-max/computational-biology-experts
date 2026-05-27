# Rahul Satija — Heuristics

1. Use SCTransform instead of log-normalization for variable sequencing depth.
2. Integrate before clustering when combining datasets from different experiments.
3. Use WNN for multimodal data — don't analyze modalities separately.
4. Validate integration with known biology (known cell types should cluster together).
5. Use Azimuth for automated annotation — manual annotation is inconsistent.
6. Sketch for datasets >500,000 cells.
7. Test multiple clustering resolutions and validate with marker genes.
8. Never interpret UMAP distances as biological distances.
