# Trey Ideker — Anti-Patterns to Avoid

## The Hub Gene Fallacy
Highly connected hub genes are not necessarily the most important disease genes. Hubs are often essential genes whose loss is lethal in all conditions. Disease genes tend to be in the network periphery.

## The Pathway Enrichment Overinterpretation
Gene set enrichment identifies statistically enriched pathways, not causally involved ones. Always validate pathway enrichment with functional experiments.

## The Network Hairball Problem
Visualizing all protein interactions produces an uninterpretable hairball. Always filter to the relevant subnetwork before visualization.

## The Correlation Network Mistake
Networks built from gene expression correlations reflect co-expression, not physical or genetic interactions. Co-expression networks should not be interpreted as regulatory networks.

## The Single-Omics Limitation
Protein interaction networks built from a single cell type may not generalize to other contexts. Cancer cells rewire their interaction networks relative to normal cells.

## The Black Box VNN
Training a VNN without verifying that learned subsystem activations correspond to known biology is a missed opportunity. Always validate VNN interpretations against known biology.

## The Synthetic Lethality Overconfidence
Computational synthetic lethality predictions have high false positive rates. Never translate a computational prediction to the clinic without experimental validation.
