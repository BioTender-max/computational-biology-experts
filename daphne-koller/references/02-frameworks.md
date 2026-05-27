# Daphne Koller — Analytical Frameworks

## Probabilistic Graphical Models Framework
**When to use:** Any problem involving uncertainty, incomplete data, or complex dependencies.
**Components:** Graph structure (conditional independence) + parameters (CPDs/potentials) + inference algorithm + learning procedure.
**Bayesian networks:** Directed acyclic graphs; encode causal/generative structure; efficient for sparse dependencies.
**Markov networks:** Undirected graphs; encode symmetric dependencies; natural for spatial/image models.

## The Three-Layer Drug Discovery Framework (insitro)
**Layer 1 — Disease model:** iPSC-derived cells that recapitulate disease biology.
**Layer 2 — Phenotypic readout:** High-content imaging capturing morphological fingerprints.
**Layer 3 — ML prediction:** Models trained on systematic perturbation data to predict drug response.
Each layer must be validated independently before the system can be trusted end-to-end.

## The Data Generation Framework
**Step 1:** Define the biological question precisely (what phenotype, what perturbation, what cell type).
**Step 2:** Design the experimental system to generate systematic, controlled data.
**Step 3:** Validate the experimental system with positive and negative controls.
**Step 4:** Scale data generation to the volume needed for ML.
**Step 5:** Train and validate ML models on held-out data from independent experiments.

## The Inference Framework
**Observation:** What data do we have? (gene expression, imaging, clinical)
**Latent variables:** What do we want to infer? (regulatory state, disease mechanism, drug response)
**Model:** What assumptions connect observations to latent variables? (PGM structure)
**Algorithm:** How do we compute the posterior? (BP, variational, MCMC)
**Validation:** Does the posterior make biological sense?

## The Uncertainty Quantification Framework
**Aleatoric uncertainty:** Irreducible noise in the data (stochastic gene expression).
**Epistemic uncertainty:** Model uncertainty due to limited data (reducible with more data).
**Calibration:** Does P(correct | confidence=p) ≈ p? Use reliability diagrams and ECE.
**Decision threshold:** Set based on the cost of false positives vs. false negatives in the specific application.
