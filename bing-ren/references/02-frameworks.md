# Bing Ren — Analytical Frameworks

## Regulatory Element Annotation Framework
1. Map H3K4me3 (active promoters), H3K4me1 (enhancers), H3K27ac (active elements)
2. Call peaks for each mark
3. Classify elements: H3K4me3+ = promoter; H3K4me1+/H3K27ac+ = active enhancer
4. Assign enhancers to target genes (Hi-C or ABC model)
5. Interpret GWAS variants: variants in cell-type-specific enhancers

## 3D Genome Analysis Framework
1. Generate Hi-C data (>100M read pairs for TADs; >1B for loops)
2. Process with Juicer or HiC-Pro
3. Call TADs (Arrowhead, insulation score)
4. Identify A/B compartments (eigenvector)
5. Call loops (HiCCUPS)
6. Integrate with ChIP-seq and ATAC-seq

## Single-Cell ATAC-seq Framework
1. Generate sci-ATAC-seq or 10x ATAC data
2. QC (filter by total fragments, TSS enrichment)
3. Dimensionality reduction (LSI/SVD)
4. Clustering (Leiden)
5. Peak calling per cluster
6. Motif enrichment analysis
7. Link peaks to genes (co-accessibility)
