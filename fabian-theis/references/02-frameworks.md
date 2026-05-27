# Fabian Theis — Analytical Frameworks

## Standard scRNA-seq Analysis Pipeline (scanpy)
1. Quality control: filter cells (n_genes, n_counts, pct_mito), filter genes
2. Normalization: total-count normalize, log1p transform
3. Feature selection: highly variable genes (HVGs)
4. Dimensionality reduction: PCA → neighbors graph → UMAP
5. Clustering: Leiden community detection
6. Annotation: marker gene analysis, reference mapping (scArches)
7. Differential expression: Wilcoxon, DESeq2

## RNA Velocity Analysis Framework (scVelo)
1. Quantify spliced and unspliced counts (STARsolo, alevin)
2. Filter and normalize (scv.pp.filter_and_normalize)
3. Compute moments (scv.pp.moments)
4. Fit kinetic model (scv.tl.velocity, mode='dynamical')
5. Compute velocity graph (scv.tl.velocity_graph)
6. Visualize velocity embedding (scv.pl.velocity_embedding_stream)
7. Validate against known biology

## Cell Fate Mapping Framework (CellRank)
1. Compute velocity kernel (VelocityKernel)
2. Combine with connectivity kernel
3. Identify terminal states (GPCCA)
4. Compute fate probabilities (absorption probabilities)
5. Identify driver genes for each fate transition
6. Validate with pseudotime and experimental data

## Batch Integration Framework (scVI)
1. Setup AnnData with batch key and count layer
2. Train scVI model (n_latent=30, max_epochs=400)
3. Extract batch-corrected latent representation
4. Use latent representation for downstream analysis
5. Validate: check that biological variation is preserved
6. Differential expression using scVI's posterior sampling
