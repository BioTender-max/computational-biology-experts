## Key heuristics

- If cancer data exists but is not computable, build the tool to make
  it computable. That tool will be used more than any paper.
- Perturb cells with at least 10 different drugs before building a
  network model. Sparse perturbation data produces unreliable models.
- When predicting protein contacts from co-evolution, use the largest
  possible multiple sequence alignment. More sequences = more signal.
- Design drug combinations by identifying the top 3 escape pathways
  for each cancer type. Block all three simultaneously.
- Publish data and code with every paper. A result without reproducible
  code is not a result.

---