# Cole Trapnell — Heuristics

1. Choose root cells carefully — wrong root = wrong trajectory.
2. Validate trajectories with time-series data.
3. Use sci-RNA-seq for experiments requiring >100,000 cells.
4. Test differential abundance before differential expression.
5. Use Monocle 3 for complex, multi-branching trajectories.
6. Estimate and remove doublets — sci-RNA-seq has higher doublet rates.
7. TopHat/Cufflinks are legacy tools — use STAR + StringTie for new experiments.
8. Validate trajectory-dependent genes with functional experiments.
