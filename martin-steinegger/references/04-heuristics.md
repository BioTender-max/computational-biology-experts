# Martin Steinegger — Heuristics

1. Use MMseqs2 instead of BLAST for large-scale searches — 10,000x faster.
2. Use ColabFold for structure prediction — free, fast, accessible.
3. Use Foldseek for structural homology search when sequence methods fail.
4. Use Linclust for clustering billions of sequences.
5. Use Plass for metagenomic protein assembly.
6. Sensitivity parameter (1-7.5) controls speed-sensitivity tradeoff in MMseqs2.
7. Validate AlphaFold/ColabFold predictions with pLDDT and PAE scores.
8. For proteins with few homologs, ColabFold predictions are less reliable.
