# Cole Trapnell — Anti-Patterns

## Pseudotime Causality Fallacy
Pseudotime ordering does not prove that cells are transitioning between states. Causal claims require perturbation experiments.

## Root Cell Sensitivity
Pseudotime is highly sensitive to root cell choice. Always validate with known biology.

## Trajectory Overfitting
Monocle can fit complex trajectories to noise. Validate trajectory structure with biological knowledge.

## sci-RNA-seq Doublet Rate
Combinatorial indexing has higher doublet rates (~5-10%). Always remove doublets before analysis.

## Differential Expression Along Trajectory Pitfall
Simple linear regression is inappropriate for non-linear expression patterns. Use GAMs or splines.
