# Heuristics — Barbara Engelhardt

## Practical Rules for Probabilistic ML in Genomics

1. **Always model confounders**: Unmodeled batch effects and hidden covariates inflate false discovery rates. Use PEER or similar methods.

2. **Quantify uncertainty**: Report credible intervals, not just point estimates. Uncertainty is information.

3. **Use causal models for interventions**: Predictive models trained on observational data cannot predict the effects of interventions without causal assumptions.

4. **Regularize in high dimensions**: With more features than samples, regularization and principled model selection are essential.

5. **Validate on independent cohorts**: Models must be validated on data from different batches, institutions, or time periods.

6. **Collaborate with domain experts**: Statistical models are only useful if they address real biological or clinical questions.
