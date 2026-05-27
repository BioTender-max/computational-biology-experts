# Rahul Satija — Analytical Frameworks

## Standard Seurat Pipeline
1. QC (filter cells by nFeature, nCount, pct.mt)
2. Normalization (SCTransform or NormalizeData)
3. Feature selection (FindVariableFeatures)
4. Dimensionality reduction (PCA → UMAP)
5. Clustering (FindNeighbors → FindClusters)
6. Annotation (marker genes, Azimuth)

## Integration Framework (Seurat v3)
1. Find variable features in each dataset
2. Run CCA to find shared dimensions
3. Identify anchor cells (mutual nearest neighbors in CCA space)
4. Correct batch effects using anchors
5. Downstream analysis on integrated embedding

## WNN Multimodal Framework
1. Compute cell-specific modality weights
2. Build WNN graph weighted by modality weights
3. Cluster and visualize using WNN graph
4. Annotate using both modalities

## Reference Mapping Framework (Azimuth)
1. Build high-quality reference atlas
2. Map query dataset onto reference using transfer learning
3. Transfer cell type labels and embeddings
4. Identify novel cell states not in reference
