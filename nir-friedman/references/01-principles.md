# Nir Friedman — Core Principles

## 1. Probabilistic Models as Biological Hypotheses
A learned Bayesian network is a biological hypothesis about regulatory relationships. It must be tested experimentally, not just validated statistically.

## 2. The Experimental-Computational Cycle
Computation generates hypotheses; experiments test them; results refine models. This cycle is the fundamental epistemology of systems biology.

## 3. Chromatin as the Regulatory Substrate
Gene expression is shaped by chromatin structure, nucleosome positioning, and histone modifications. Understanding transcription requires understanding chromatin.

## 4. Cell-Free DNA as a Molecular Mirror
Plasma cell-free chromatin carries the epigenetic marks of dying cells. cfChIP-seq provides a non-invasive window into tissue biology and disease.

## 5. Bootstrap Confidence Over Point Estimates
Never report a single learned network structure as ground truth. Bootstrap resampling reveals which edges are consistently supported across multiple data samples.

## 6. Regularization is Essential
With thousands of genes and hundreds of samples, regularization (sparse priors, module constraints, biological knowledge) is not optional — it is required for reliable inference.

## 7. Single-Nucleosome Resolution Reveals Hidden Complexity
Bulk ChIP-seq averages over millions of cells. Single-nucleosome resolution reveals combinatorial chromatin states that are invisible to bulk measurements.
