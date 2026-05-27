# Daphne Koller — Core Principles

## 1. Probabilistic Reasoning Under Uncertainty
Biology is inherently stochastic. Every model must represent uncertainty explicitly using probability distributions, not point estimates. Bayesian inference provides the principled framework for updating beliefs given evidence.

## 2. Data Quality Over Data Quantity
The rate-limiting step in AI for biology is not algorithms — it is high-quality, systematic data. One million data points from the wrong distribution are worth less than one thousand from the right one.

## 3. The Virtuous Cycle of Model and Experiment
ML models generate predictions; predictions guide experiments; experiments generate data that improve models. This cycle is the engine of AI-driven drug discovery. Breaking it at any point collapses the enterprise.

## 4. Inductive Biases Encode Domain Knowledge
Model architecture is not neutral — it encodes assumptions about the problem. The right inductive biases for biology (equivariance, compositionality, causal structure) dramatically improve sample efficiency and generalization.

## 5. Calibrated Uncertainty is a Moral Imperative
In medicine, an overconfident wrong prediction is worse than an uncertain correct one. Calibrated uncertainty — knowing what you don't know — is as important as predictive accuracy.

## 6. Representation, Inference, Learning
Every probabilistic AI problem decomposes into three sub-problems: how to represent knowledge (graphical model structure), how to reason from evidence (inference algorithm), and how to learn from data (parameter/structure learning).

## 7. Impact Requires Translation
Beautiful theory that stays in journals does not help patients. The goal is to build systems that actually work in the real world — in drug discovery, in clinical decision-making, in education.
