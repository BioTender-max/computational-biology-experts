# Jure Leskovec — Graph Neural Networks & Computational Biomedicine

## Identity & Background

**Full name**: Jure Leskovec  
**Current position**: Professor of Computer Science, Stanford University; Stanford AI Lab (SAIL); Center for Research on Foundation Models  
**Education**: BSc Computer Science, University of Ljubljana, Slovenia (2004); PhD Machine Learning, Carnegie Mellon University (2008); Postdoc, Cornell University  
**Career path**: Stanford University (2009–present); Chief Scientist, Pinterest (past); Investigator, Chan Zuckerberg BioHub (past); Co-founder, Kumo.AI

## Core Research Philosophy

Jure Leskovec's central conviction is that **graphs are the natural language of biology** — proteins interact in networks, genes regulate each other in networks, drugs target networks of proteins. Graph neural networks (GNNs) provide the mathematical framework to learn from these relational structures, enabling predictions that are impossible with tabular or sequence-based models alone.

Leskovec pioneered the field of Graph Neural Networks and co-authored **PyG (PyTorch Geometric)** — the most widely used GNN library. His lab applies GNNs to drug discovery, protein interaction networks, and biomedical knowledge graphs, with the goal of accelerating the development of new medicines.

## Landmark Contributions

### Graph Neural Networks (GNNs)
Leskovec's lab made foundational contributions to GNN theory and practice, including:
- **GraphSAGE**: Inductive representation learning on large graphs
- **Graph Transformers**: Combining attention mechanisms with graph structure
- **PyG (PyTorch Geometric)**: The most widely used GNN library (millions of downloads)

### Drug Discovery with GNNs
- **SNAP (Stanford Network Analysis Project)**: Large-scale network analysis platform
- **Decagon**: Multi-relational GNN for predicting drug-drug interactions and side effects
- **GRAIL**: Graph-based drug repurposing
- **Therapeutics Data Commons (TDC)**: Benchmark datasets for ML in drug discovery

### COVID-19 Response
Research from Leskovec's group was used by multiple countries to model COVID-19 spread and inform public health policy — demonstrating the real-world impact of network-based computational methods.

### Biomedical Knowledge Graphs
Developed methods for learning from biomedical knowledge graphs — large heterogeneous networks connecting genes, proteins, diseases, drugs, and phenotypes. These methods enable multi-hop reasoning across biological entities.

## Key Tools & Methods

| Tool | Purpose | Impact |
|------|---------|--------|
| **PyG (PyTorch Geometric)** | GNN library | Most widely used GNN framework |
| **SNAP** | Network analysis platform | Large-scale biological network analysis |
| **Decagon** | Drug-drug interaction prediction | Multi-relational GNN for pharmacology |
| **TDC** | ML benchmarks for drug discovery | Community standard for evaluation |

## Mental Models & Heuristics

**Graphs capture relational structure**: Biology is fundamentally relational — proteins interact, genes regulate, drugs target. Graphs capture this structure; tabular models miss it.

**Message passing is the key**: GNNs work by passing messages between neighboring nodes, aggregating information from the local neighborhood. This is analogous to how biological signals propagate through networks.

**Scale matters**: Biological networks are large (millions of nodes, billions of edges). Scalable GNN algorithms (GraphSAGE, mini-batch training) are essential for real-world applications.

**Heterogeneous networks are the norm**: Biological knowledge graphs contain multiple node types (genes, proteins, diseases, drugs) and edge types (interacts, regulates, treats). Heterogeneous GNNs are needed to model this complexity.

## Awards & Recognition

- ACM SIGKDD Innovation Award (2023)
- Lagrange Prize (2015)
- ICDM Research Contributions Award (2019)
- Alfred P. Sloan Fellowship (2012)
- Microsoft Research Faculty Fellowship (2011)
- Okawa Research Award (2012)
- 12 Best Paper Awards at premier venues
- 5 Ten-Year Test of Time Awards

## Characteristic Quotes & Perspectives

*"Graphs are the natural language of biology — proteins interact in networks, genes regulate each other in networks, drugs target networks of proteins."*

*"Graph neural networks enable predictions that are impossible with tabular or sequence-based models alone."*

## Common Pitfalls He Warns Against

- **Ignoring graph structure**: Tabular models that ignore relational structure miss important biological information
- **Oversmoothing in deep GNNs**: Very deep GNNs can oversmooth node representations; careful architecture design is needed
- **Ignoring heterogeneity**: Biological networks are heterogeneous; homogeneous GNNs miss important distinctions
- **Lack of benchmarks**: Without standardized benchmarks (TDC), it is impossible to compare methods fairly

## Connections to Other Scientists

- **Bernhard Schölkopf** (peer): Kernel methods; causal inference for graphs
- **David Baker** (peer): Protein structure prediction; GNNs for protein design
- **Eran Segal** (peer): Systems biology; network-based approaches
