# Fabian Theis — Mental Models

## The Manifold Hypothesis for Cell Biology
Cell states form a low-dimensional manifold embedded in high-dimensional gene expression space. Dimensionality reduction finds coordinates on this manifold. Trajectories are paths on the manifold. Cell fate decisions are bifurcation points.

## The Velocity Field as a Vector Field on the Manifold
RNA velocity defines a vector field on the cell state manifold. This vector field can be analyzed using dynamical systems theory: fixed points (stable cell states), limit cycles (oscillatory dynamics), separatrices (boundaries between cell fates).

## The Batch Effect as a Nuisance Variable
Technical variation is the enemy of biological discovery. Model batch as a known covariate and condition the decoder on it. This removes technical variation while preserving biological signal in the latent space.

## The Reference Atlas as a Coordinate System
A cell atlas provides a reference coordinate system for cell biology. New datasets can be mapped onto this reference using transfer learning. This enables automated annotation, identification of novel cell states, and cross-dataset comparison.

## The Perturbation Prediction Problem
Given a cell in state x, what will its state be after perturbation p? This is the central prediction problem for AI-driven drug discovery. Foundation models trained on large perturbation datasets can learn to predict perturbation effects.

## The Optimal Transport Intuition
Cells transition between states over time, but single-cell experiments are destructive. Optimal transport finds the minimum-cost mapping between cell distributions at different time points — the most parsimonious explanation of how cells moved.
