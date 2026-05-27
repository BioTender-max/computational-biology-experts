# Daphne Koller — Heuristics & Rules of Thumb

1. **Start with the simplest model.** Add complexity only when simpler models are demonstrably insufficient. Occam's razor applies to biology.

2. **Data first, model second.** Before choosing an algorithm, ask: do I have the right data? The best algorithm on the wrong data will fail.

3. **Validate on truly independent data.** A model that achieves 95% accuracy on held-out data from the same experiment may fail on data from a different lab. Always evaluate on genuinely independent data.

4. **Report uncertainty, not just predictions.** Every prediction should come with a confidence interval or probability distribution. A point estimate without uncertainty is not a scientific result.

5. **The graph structure is a hypothesis.** A learned Bayesian network structure is a hypothesis about conditional independence, not a proven causal map. Every edge requires experimental validation.

6. **Calibrate before deploying.** Check that your model's confidence scores are calibrated (reliability diagram). Miscalibrated models are dangerous in medical applications.

7. **Biological knowledge is a prior.** Don't ignore known biology when building models. Protein interaction databases, pathway annotations, and evolutionary conservation are informative priors.

8. **The feedback loop is the product.** In AI-driven drug discovery, the model-experiment feedback loop is more important than any single model. Design the loop before designing the model.

9. **Negative results are data.** A failed experiment that contradicts a model prediction is as valuable as a successful one. It tells you where the model is wrong.

10. **Interpretability matters in medicine.** A black-box model that a clinician cannot understand will not be adopted. Build interpretability in from the start.
