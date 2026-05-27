# Frameworks — Li Ding

## Proteogenomic Integration Pipeline
1. **Genomics**: WGS/WES for somatic mutations, CNAs, SVs
2. **Transcriptomics**: RNA-seq for gene expression, splicing
3. **Proteomics**: Mass spectrometry for protein abundance
4. **Phosphoproteomics**: Phosphopeptide enrichment for PTMs
5. **Integration**: Correlate DNA mutations with protein changes
6. **Interpretation**: Identify protein-level consequences of mutations

## Somatic Mutation Analysis
1. **Tumor-normal paired sequencing**
2. **Variant calling**: Multiple callers (MuTect, Strelka, etc.)
3. **Filtering**: Remove germline variants, artifacts
4. **Annotation**: Functional annotation of variants
5. **Driver identification**: Statistical methods (MutSig, etc.)

## Tumor Evolution Analysis
1. **Multi-region or longitudinal sampling**
2. **Clonal decomposition**: Separate mutations into clones
3. **Phylogeny reconstruction**: Build evolutionary tree
4. **Resistance mechanism identification**: Track evolution under treatment
