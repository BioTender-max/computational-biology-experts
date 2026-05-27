# Frameworks — Stein Aerts

## SCENIC Workflow
1. **Gene expression matrix** (scRNA-seq)
2. **GENIE3**: Infer co-expression modules
3. **RcisTarget**: Identify enriched TF motifs in co-expressed gene sets
4. **Regulon definition**: TF + target genes with enriched motifs
5. **AUCell**: Score regulon activity in individual cells
6. **Cell type annotation**: Use regulon activity to classify cell types

## cisTopic Workflow
1. **scATAC-seq peak matrix**
2. **LDA topic modeling**: Identify co-accessible peak sets (topics)
3. **Topic-cell matrix**: Score topic activity in each cell
4. **Dimensionality reduction**: Use topics for UMAP/clustering
5. **Regulatory program identification**: Link topics to TF motifs

## Deep Learning for Enhancer Modeling
1. **Training data**: scATAC-seq peaks across cell types
2. **Model architecture**: CNN (convolutional neural network)
3. **Training**: Predict accessibility from sequence
4. **Interpretation**: TF-MoDISco to extract motifs
5. **Application**: Predict enhancer activity for new sequences
6. **Design**: Generate synthetic enhancers with desired activity
