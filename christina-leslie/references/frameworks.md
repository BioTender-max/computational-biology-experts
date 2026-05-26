# Christina Leslie — Conceptual Frameworks

## Framework 1: String Kernel Methods for Biological Sequences
**Problem**: How do you classify biological sequences (proteins, DNA) using machine learning when the sequences have variable length and complex structure?

**Solution**: String kernels — functions that measure similarity between sequences based on shared subsequences (k-mers), counted with up to m mismatches. These kernels can be used with SVMs for discriminative classification.

**Key components**:
- Spectrum kernel: counts exact k-mer matches
- Mismatch kernel: counts k-mer matches with up to m mismatches
- Mismatch tree: efficient data structure for computing the mismatch kernel

**Key insight**: The mismatch kernel captures sequence similarity without requiring alignment, and can be computed efficiently using a mismatch tree data structure.

**Applications**: Protein remote homology detection, transcription factor binding site prediction, regulatory sequence classification.

---

## Framework 2: Discriminative Models for Gene Regulation
**Problem**: How do you learn the sequence preferences of transcription factors from ChIP-seq data?

**Approach**: Train discriminative models (string kernel SVMs, later deep learning) to distinguish TF-bound sequences from unbound sequences. This is a prediction task, not a motif discovery task.

**Key insight**: Some TFs recognize cell-type-specific sequence signals, due to differences in the composition of the TF binding complex. Discriminative models can capture these subtle, context-dependent preferences.

**Tools**: SeqGL (sequence-based group lasso), BindSpace (embedding space for TF binding), BindVAE (variational autoencoder for de novo motif discovery).

---

## Framework 3: 3D Genome-Aware Gene Regulation (GraphReg)
**Problem**: Distal enhancers regulate gene expression through 3D chromatin interactions, but most models only use 1D epigenomic data.

**Solution**: GraphReg — a graph attention network that exploits 3D interactions from chromosome conformation capture (Hi-C) data to predict gene expression from epigenomic data or DNA sequence.

**Architecture**:
1. Represent genomic loci as nodes in a graph
2. Use Hi-C data to define edges (chromatin interactions)
3. Apply graph attention network to propagate information across the graph
4. Predict gene expression from the aggregated node features

**Key insight**: By modeling the connectivity of distal elements and promoters, GraphReg more faithfully models gene regulation than dilated CNNs.

**Validation**: Feature attribution accurately identifies functional enhancers, validated by CRISPRi-FlowFISH and TAP-seq assays.

---

## Framework 4: microRNA Competition and ceRNA Networks
**Problem**: microRNAs regulate gene expression post-transcriptionally, but the competitive dynamics between miRNAs and their targets are poorly understood.

**Contribution**: First systems-level analyses of competition between microRNAs and between target transcripts (ceRNA hypothesis).

**Method**: mirSVR — SVM-based microRNA target prediction using sequence and structural features. Applied genome-wide to identify ceRNA networks.
