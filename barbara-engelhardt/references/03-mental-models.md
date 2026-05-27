# Mental Models — Barbara Engelhardt

## The Confounder Problem
Gene expression data is full of hidden confounders — batch effects, cell cycle, technical variation. Latent factor models like PEER identify and remove these confounders, revealing true biological signal.

## The Causal Graph
Biological systems are causal: genes regulate other genes, proteins interact, drugs perturb pathways. Causal models capture these relationships; correlational models miss them.

## The Uncertainty Landscape
Every prediction has uncertainty. Bayesian models quantify this uncertainty, enabling users to distinguish confident predictions from uncertain ones.

## The Clinical Decision Problem
Clinical decision-making is a sequential process: observe patient state, choose action, observe outcome, repeat. Reinforcement learning is the natural framework for this problem.
