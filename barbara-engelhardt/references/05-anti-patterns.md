# Anti-Patterns — Barbara Engelhardt

## What to Avoid in Probabilistic ML for Genomics

### Ignoring Confounders
Unmodeled batch effects and hidden covariates inflate false discovery rates in genomics. Always model and remove confounders.

### Point Estimates Without Uncertainty
Models that don't quantify uncertainty mislead users about confidence. Always report credible intervals or posterior distributions.

### Correlation vs. Causation
Predictive models trained on observational data cannot be used to predict the effects of interventions without causal assumptions.

### Overfitting in High Dimensions
With more features than samples, regularization and principled model selection are essential. Cross-validation is not sufficient for high-dimensional data.

### Ignoring Clinical Context
Statistical models developed without clinical input often fail to address real clinical problems. Always collaborate with domain experts.
