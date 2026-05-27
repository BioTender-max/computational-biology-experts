# Mental Models — Anshul Kundaje

## The Regulatory Grammar
Gene regulation is governed by a grammar — rules about which TF motifs, in what combinations and orientations, drive expression in which cell types. Deep learning models learn this grammar from data.

## The Sequence-to-Function Map
DNA sequence → TF binding → chromatin accessibility → gene expression. Each step in this map can be modeled computationally; the full map connects genotype to phenotype.

## The Variant Effect Landscape
Every genetic variant exists in a landscape of regulatory effects. Most variants have no effect; some affect TF binding; fewer affect gene expression; fewer still affect disease. Computational models navigate this landscape.

## The Interpretability Imperative
A deep learning model is a hypothesis about the regulatory grammar. TF-MoDISco extracts this hypothesis in human-interpretable form — as sequence motifs and their interactions.
