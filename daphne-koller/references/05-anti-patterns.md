# Daphne Koller — Anti-Patterns to Avoid

## The Correlation-Causation Conflation
Bayesian networks learned from observational data encode conditional independence, not causation. Never claim that an edge in a learned BN represents a causal regulatory relationship without interventional data or strong causal assumptions.

## The Overfit Regulatory Network
Learning a fully connected BN over 20,000 genes from 100 samples will overfit catastrophically. Always regularize (sparse priors, module constraints, biological knowledge). Control the number of parameters relative to sample size.

## The Single-Model Fallacy
Committing to a single MAP graph structure ignores model uncertainty. Report edge confidence from bootstrap or Bayesian model averaging, not just presence/absence.

## The Benchmark Overfitting Trap
ML models for biology are routinely evaluated on benchmarks that don't reflect real-world deployment. A model that achieves 95% accuracy on held-out cell lines from the same experiment may fail on cell lines from a different lab. Always evaluate on truly independent data.

## The Data-Free Prior
Using uninformative priors when biological knowledge is available wastes information. Protein interaction databases, pathway annotations, and evolutionary conservation are all informative priors. Ignoring them is leaving signal on the table.

## The Phenotype-Genotype Shortcut
Predicting drug response from genotype alone ignores cellular context. The same mutation has different effects in different cell types, developmental stages, and environmental conditions. Models must account for cellular context.

## The Overconfident Prediction
Deploying a model without calibration in a medical context is dangerous. Always check calibration and report uncertainty. An overconfident wrong prediction can lead to patient harm.
