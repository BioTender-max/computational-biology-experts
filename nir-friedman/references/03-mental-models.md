# Nir Friedman — Mental Models

## The Regulatory Network as a Causal Graph
Gene regulatory networks encode causal relationships, not just correlations. Distinguishing correlation from causation requires interventional data (knockouts) or strong causal assumptions.

## The Chromatin State Machine
Chromatin exists in discrete states defined by combinations of histone modifications. Transitions between states are regulated processes underlying differentiation, response to signals, and disease.

## The Liquid Biopsy Information Hierarchy
cfDNA mutations → cfDNA methylation → cfChIP-seq → cfRNA → exosomes. Each modality provides different information about cell state. cfChIP-seq uniquely provides epigenomic information about active regulatory elements.

## The Bootstrap Confidence Principle
Never report a single learned network structure as ground truth. Bootstrap resampling reveals which edges are consistently supported. An edge with 80% bootstrap confidence is much more reliable than one with 20%.

## The Hierarchy of Biological Regulation
DNA sequence → chromatin accessibility → histone modifications → TF binding → mRNA → protein. Probabilistic models must integrate information across all these scales.

## The Experimental-Computational Cycle
Computation generates hypotheses → experiments test them → results refine models. This cycle is the fundamental epistemology of systems biology. Breaking it produces less reliable knowledge.
