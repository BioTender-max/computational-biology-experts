# Anti-Patterns — Jure Leskovec

## What to Avoid in GNNs for Biology

### Ignoring Graph Structure
Tabular models that ignore relational structure miss important biological information. Always consider whether a graph representation is appropriate.

### Oversmoothing in Deep GNNs
Very deep GNNs can oversmooth node representations, making all nodes look similar. Use skip connections or limit depth.

### Ignoring Heterogeneity
Biological networks are heterogeneous. Homogeneous GNNs that treat all nodes and edges the same miss important distinctions.

### Lack of Benchmarks
Without standardized benchmarks, it is impossible to compare methods fairly. Always evaluate on established benchmarks.

### No Experimental Validation
GNN predictions are hypotheses. Always validate top predictions experimentally.
