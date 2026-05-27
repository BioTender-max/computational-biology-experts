# Frameworks — Barbara Engelhardt

## PEER (Probabilistic Estimation of Expression Residuals)
1. **Input**: Gene expression matrix + known covariates
2. **Latent factor model**: Identify hidden factors explaining residual variation
3. **Factor removal**: Regress out latent factors to remove confounders
4. **Output**: Corrected expression matrix for eQTL mapping

## Gaussian Process Latent Variable Model (GPLVM)
1. **Input**: High-dimensional single-cell data
2. **Latent space**: Learn low-dimensional embedding
3. **GP prior**: Smooth, non-linear mapping from latent to observed space
4. **Uncertainty**: Quantify uncertainty in embedding
5. **Output**: Dimensionality-reduced representation with uncertainty

## Reinforcement Learning for Clinical Decision Support
1. **State**: Patient clinical variables (vitals, labs, medications)
2. **Action**: Treatment decision (drug, dose, timing)
3. **Reward**: Patient outcome (survival, recovery)
4. **Policy learning**: Learn optimal treatment policy from observational data
5. **Validation**: Evaluate policy on held-out patients
