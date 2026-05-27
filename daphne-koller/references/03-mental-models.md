# Daphne Koller — Mental Models

## The Inference Lens
Every biological question is an inference problem. Frame it as: given observations O, what is the posterior P(H|O) over hypotheses H? This forces clarity about what is observed, what is latent, and what assumptions are encoded in the model.

## The Data Quality Hierarchy
1. Systematic, controlled perturbation data (highest value)
2. Large-scale observational data (high volume, confounded)
3. Small-scale mechanistic data (high quality, low throughput)
4. Literature-derived data (noisy, biased)
Train ML models on data from the top of this hierarchy.

## The Inductive Bias Principle
ML models learn from data + inductive biases. The right inductive biases for biology: equivariance to cell identity, compositionality of gene effects, causal structure of interventions. Choosing the architecture is choosing the inductive biases.

## The Virtuous vs. Vicious Cycle
Virtuous: Good data → good model → good predictions → targeted experiments → better data.
Vicious: Poor data → overfit model → wrong predictions → uninformative experiments → same poor data.
The difference between successful and failed AI-in-biology efforts traces to this cycle.

## The Uncertainty Quantification Imperative
A confident wrong answer is worse than an uncertain right answer. In drug discovery, overconfident predictions lead to expensive failed experiments. Calibrated uncertainty is not a luxury — it's a requirement.

## The Biological Foundation Model Vision
Just as LLMs learn universal representations of language, biological foundation models can learn universal representations of cell biology. The key: massive, diverse, high-quality single-cell data + the right architecture + careful fine-tuning for specific tasks.
