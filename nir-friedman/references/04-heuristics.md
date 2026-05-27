# Nir Friedman — Heuristics & Rules of Thumb

1. **Validate every computational edge experimentally.** A Bayesian network edge is a hypothesis, not a fact. Require experimental validation before claiming regulatory relationships.

2. **Use bootstrap confidence.** Report edge confidence from bootstrap resampling, not just presence/absence. Edges with <50% bootstrap confidence are likely spurious.

3. **Regularize aggressively.** With 1,000 genes and 100 samples, you're severely underpowered. Use sparse priors, module constraints, or biological knowledge to regularize.

4. **Prefer continuous BN models when sample size permits.** Discretization loses information and introduces artifacts. Gaussian BNs or conditional Gaussian BNs are more principled.

5. **Control for multiple testing.** When learning networks over thousands of genes, use permutation-based FDR correction or Bayesian approaches that naturally penalize complexity.

6. **Validate cfChIP-seq deconvolution with orthogonal methods.** Tissue-of-origin inference from cfChIP-seq should be validated with cell-type-specific markers or orthogonal liquid biopsy modalities.

7. **Process cfDNA samples rapidly.** Cell-free DNA degrades quickly. Rapid processing (EDTA tubes, low centrifugation speed, immediate freezing) is essential for reliable results.

8. **Spend time in the wet lab.** The best computational biologists understand the experiments that generate their data. Spend at least 30% of time understanding the biology.
