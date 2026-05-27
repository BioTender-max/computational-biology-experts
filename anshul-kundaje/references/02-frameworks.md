# Frameworks — Anshul Kundaje

## BPNet Workflow
1. **Training data**: ChIP-seq profiles for TFs at base resolution
2. **Model architecture**: Dilated CNN (BPNet)
3. **Training**: Predict TF binding profiles from sequence
4. **Interpretation**: TF-MoDISco to extract sequence motifs
5. **Application**: Predict TF binding for new sequences
6. **Variant scoring**: Predict effect of SNPs on TF binding

## ChromBPNet Workflow
1. **Training data**: scATAC-seq or bulk ATAC-seq profiles
2. **Model architecture**: ChromBPNet (bias-corrected BPNet)
3. **Training**: Predict chromatin accessibility from sequence
4. **Interpretation**: Extract cell-type-specific regulatory motifs
5. **Application**: Predict accessibility for new sequences and variants

## ENCODE Pipeline
1. **Raw data**: ChIP-seq, ATAC-seq, RNA-seq FASTQ files
2. **Alignment**: BWA, STAR
3. **Peak calling**: MACS2, IDR
4. **QC**: Cross-correlation, FRiP, library complexity
5. **Output**: Reproducible peak sets, signal tracks
