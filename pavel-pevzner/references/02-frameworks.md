# Pavel Pevzner — Conceptual Frameworks

## Framework 1 — De Bruijn Graphs for Genome Assembly
A de Bruijn graph represents all k-mers in reads as edges, with (k-1)-mers as nodes. Assembly = finding an Eulerian path (linear time), not a Hamiltonian path (NP-hard).
**Tools**: SPAdes, Velvet, ABySS

## Framework 2 — The Repeat Graph for Long-Read Assembly
Long reads span most repeats. The repeat graph collapses repeat regions into single nodes; long reads resolve the graph.
**Tools**: Flye, Raven

## Framework 3 — The Breakpoint Graph for Genome Rearrangements
Genome rearrangements are operations on a breakpoint graph. Minimum rearrangements = minimum operations to transform one graph into another.
**Tools**: GRIMM, MAUVE

## Framework 4 — De Novo Peptide Sequencing
Mass spectrometry spectrum → spectrum graph → path finding. Same algorithmic structure as genome assembly.
**Tools**: PEAKS, NOVOR

## Framework 5 — Antibiotic Discovery by Genome Mining
NRPS/PKS gene clusters produce antibiotics. Computational genome mining identifies clusters and predicts antibiotic structures.
**Tools**: antiSMASH, PRISM
