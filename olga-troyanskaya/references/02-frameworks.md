# Frameworks — Olga Troyanskaya

## Bayesian Data Integration
1. **Data collection**: Gene expression, protein interactions, sequence features, etc.
2. **Prior specification**: Define prior probabilities for gene function
3. **Likelihood computation**: Compute likelihood of each data type given gene function
4. **Posterior computation**: Combine prior and likelihoods using Bayes' theorem
5. **Prediction**: Use posterior to predict gene function

## DeepSEA/Sei Workflow
1. **Input**: DNA sequence (1kb window around variant)
2. **Model**: Deep CNN trained on chromatin accessibility data
3. **Prediction**: Predict chromatin effects across hundreds of cell types
4. **Variant scoring**: Compare predictions for reference and alternate alleles
5. **Prioritization**: Rank variants by predicted functional impact
