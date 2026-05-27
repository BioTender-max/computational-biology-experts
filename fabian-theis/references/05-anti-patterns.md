# Fabian Theis — Anti-Patterns to Avoid

## The Overclustering Trap
Using too high a resolution in Leiden clustering produces many small clusters that are statistically distinct but biologically meaningless. Always validate clusters with marker genes and biological knowledge.

## The UMAP Topology Fallacy
UMAP preserves local structure but distorts global topology. Distances between clusters in UMAP space are not meaningful. Never interpret UMAP distances as biological distances.

## The Batch Correction Overcorrection
Aggressive batch correction can remove real biological variation. If your biological condition of interest is confounded with batch, batch correction will remove the signal you care about.

## The Velocity Arrow Overinterpretation
RNA velocity arrows show the direction of transcriptional change, not the actual trajectory of individual cells. Always interpret velocity in the context of the full velocity field, not individual arrows.

## The Single-Dataset Conclusion
Conclusions drawn from a single dataset may not generalize. Always validate findings in independent datasets from different labs, protocols, and species.

## The Marker Gene Shortcut
Annotating cell types based on a handful of marker genes is error-prone. Use reference-based annotation (scArches, Azimuth) when possible, and validate with multiple markers.

## The Foundation Model Hype Trap
Foundation models are powerful but not magic. They are only as good as the data they're trained on. Always validate foundation model predictions with experimental data before drawing biological conclusions.
