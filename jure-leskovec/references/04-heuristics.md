# Heuristics — Jure Leskovec

## Practical Rules for GNNs in Biology

1. **Choose the right graph representation**: The choice of nodes and edges determines what information is captured. Think carefully about what biological relationships to include.

2. **Use heterogeneous GNNs for knowledge graphs**: Biological knowledge graphs have multiple node and edge types; homogeneous GNNs miss important distinctions.

3. **Avoid oversmoothing**: Very deep GNNs can oversmooth node representations. Use skip connections or limit depth.

4. **Use standardized benchmarks**: Always evaluate on TDC or other standardized benchmarks to enable fair comparison.

5. **Validate experimentally**: GNN predictions must be validated experimentally before drawing biological conclusions.
