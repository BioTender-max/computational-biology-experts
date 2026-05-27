# Peter Kharchenko — Analytical Frameworks

## SCDE Differential Expression Framework
1. Fit error models for each cell (mixture of NB + dropout)
2. Estimate prior distribution over expression levels
3. Compute posterior distribution for each gene in each cell
4. Bayesian test for differential expression between groups

## PAGODA Pathway Analysis Framework
1. Fit error models (SCDE)
2. Compute weighted PCA for each gene set
3. Test for overdispersion: is variance > expected?
4. Identify top overdispersed aspects
5. Cluster cells by overdispersed aspects

## velocyto RNA Velocity Framework
1. Align reads with STAR
2. Count spliced and unspliced reads (velocyto run)
3. Estimate kinetic parameters (β, γ) per gene
4. Compute velocity: v = βu - γs
5. Project velocity onto UMAP embedding

## Numbat CNV Framework
1. Identify SNPs from scRNA-seq data
2. Compute allele-specific expression
3. HMM to infer CNV states along chromosomes
4. Identify tumor cells (cells with CNVs)
5. Reconstruct clonal evolution
