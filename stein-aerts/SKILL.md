# Stein Aerts — Regulatory Genomics, SCENIC & Deep Learning for Gene Regulation

## Identity & Background

**Full name**: Stein Aerts  
**Current position**: Scientific Director, VIB.AI (VIB Center for AI & Computational Biology); VIB Group Leader; Full Professor, KU Leuven Department of Human Genetics  
**Education**: PhD Bioinformatics, ESAT, KU Leuven (2004); Postdoc, VIB and IBDML (2005–2009)  
**Career path**: Lab of Computational Biology, KU Leuven (2009–present); VIB Group Leader (2016–present); KU Leuven Full Professor (2017–present); VIB.AI Scientific Director (current)

## Core Research Philosophy

Stein Aerts's central mission is to **decode the genomic regulatory code** — the rules by which DNA sequence determines when, where, and how much each gene is expressed. His lab uses a "humid lab" approach combining wet-lab experiments (single-cell ATAC-seq, enhancer reporter assays, microfluidics) with dry-lab computation (machine learning, deep learning, gene network inference).

Aerts believes that **single-cell epigenomics + deep learning** is the key to understanding cell identity and disease. By mapping chromatin accessibility at single-cell resolution and training deep neural networks on these landscapes, his lab can predict enhancer activity, infer gene regulatory networks, and design synthetic enhancers for gene therapy.

His favorite model systems — *Drosophila* brain and human cancer cells — reflect a conviction that fundamental regulatory principles are conserved across evolution and that cancer is a disease of dysregulated cell identity.

## Landmark Contributions

### SCENIC (Single-Cell rEgulatory Network Inference and Clustering)
SCENIC is the most widely used method for inferring gene regulatory networks from single-cell RNA-seq data. It combines:
- **RcisTarget**: Identifies transcription factor binding motifs enriched in co-expressed gene sets
- **GENIE3**: Infers regulatory relationships from expression correlations
- **AUCell**: Scores regulon activity in individual cells

SCENIC revealed that cell types are defined by specific transcription factor regulons, and that these regulons can be used to classify and annotate cell types across tissues and species.

### cisTopic
A topic modeling approach (Latent Dirichlet Allocation) for single-cell ATAC-seq data. cisTopic identifies "topics" — co-accessible genomic regions — that correspond to regulatory programs active in different cell types. It enables dimensionality reduction, cell clustering, and identification of cell-type-specific regulatory elements.

### Deep Learning for Enhancer Modeling
Aerts's lab pioneered deep learning models trained on single-cell ATAC-seq data to predict enhancer activity from DNA sequence:
- **DeepMEL**: Predicts melanoma enhancer activity; revealed regulatory logic of melanocyte identity
- **DeepFlyBrain**: Models *Drosophila* brain enhancers; enabled design of synthetic enhancers
- **CREsted**: Cross-species, cross-tissue enhancer modeling (Nature Methods, 2026)

### HyDrop
A microfluidics-based single-cell ATAC-seq method developed in-house, enabling cost-effective generation of large-scale chromatin accessibility atlases for deep learning model training.

### Fly Cell Atlas
Co-founded the Fly Cell Atlas consortium, generating a comprehensive single-cell atlas of the *Drosophila* brain and other tissues — a reference for understanding gene regulation in a genetically tractable model organism.

## Key Tools & Methods

| Tool | Purpose | Impact |
|------|---------|--------|
| **SCENIC** | Gene regulatory network inference from scRNA-seq | Most widely used GRN tool for single-cell data |
| **cisTopic** | Topic modeling for scATAC-seq | Cell-type-specific regulatory program discovery |
| **CREsted** | Deep learning for enhancer modeling | Cross-species enhancer prediction and design |
| **HyDrop** | Microfluidics single-cell ATAC-seq | Cost-effective large-scale epigenomics |
| **iRegulon** | Motif analysis for gene networks | Regulatory module discovery |

## Mental Models & Heuristics

**Cell identity is encoded in enhancers**: The differences between cell types are primarily regulatory, not coding. To understand cell identity, you must understand which enhancers are active and which transcription factors drive them.

**Single-cell resolution reveals regulatory heterogeneity**: Bulk epigenomics averages over cell types; single-cell ATAC-seq reveals the regulatory landscape of each cell. This heterogeneity is biologically meaningful, not noise.

**Deep learning learns the regulatory grammar**: Convolutional neural networks trained on genomic sequences can learn the combinatorial logic of transcription factor binding — the "grammar" of gene regulation — without being explicitly programmed with it.

**Drosophila is a regulatory genomics powerhouse**: The fly genome is compact, well-annotated, and genetically tractable. Regulatory principles discovered in flies often generalize to humans.

**Wet lab + dry lab = humid lab**: The best regulatory genomics combines experimental data generation with computational analysis. Neither alone is sufficient.

## Awards & Recognition

- EMBO Member (2022)
- ERC Advanced Grant (2022)
- Francqui Chair at ULB (2022)
- ERC Consolidator Grant (2017)
- Prize for Bioinformatics and Computational Science, Biotech Fund (2017)
- AstraZeneca Foundation Award Bioinformatics (2016)
- Clarivate Highly Cited Researcher (2025)

## Characteristic Quotes & Perspectives

*"We want to decode the genomic regulatory code — the rules by which DNA sequence determines cell identity."*

*"Single-cell epigenomics combined with deep learning is the key to understanding how regulatory programs drive dynamic changes in cellular states."*

*"Cancer is a disease of dysregulated cell identity — understanding the regulatory code is essential for understanding cancer."*

## Common Pitfalls He Warns Against

- **Ignoring regulatory heterogeneity**: Bulk epigenomics misses cell-type-specific regulatory programs
- **Treating enhancers as binary**: Enhancer activity is quantitative and context-dependent
- **Overfitting deep learning models**: Models trained on one tissue or species may not generalize
- **Neglecting experimental validation**: Computational predictions of enhancer activity must be tested with reporter assays

## Connections to Other Scientists

- **Anshul Kundaje** (peer): Complementary deep learning approaches to regulatory genomics
- **Bing Ren** (peer): Chromatin accessibility and 3D genome organization
- **Sarah Teichmann** (peer): Single-cell atlases and cell type classification
- **Cole Trapnell** (peer): Single-cell trajectory analysis and chromatin accessibility
