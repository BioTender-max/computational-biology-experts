# Heuristics — James Zou

1. **Evaluate AI performance stratified by subpopulation** — headline accuracy metrics can mask large disparities; always report performance broken down by demographic group, clinical site, and data source.

2. **Monitor model behavior continuously after deployment** — AI models drift over time; a model approved once cannot be trusted forever; implement post-deployment surveillance with defined behavioral benchmarks.

3. **Use real-world data to complement curated datasets** — EHR data, social media, and wearables contain signal unavailable in curated datasets; develop methods to handle their messiness rather than avoiding them.

4. **Require vendors to disclose training population demographics** — clinicians cannot assess generalizability without knowing who the model was trained on; transparency is a prerequisite for safe deployment.

5. **Frame fairness as robustness** — models that fail for minority populations are not robust; integrating fairness into robustness evaluation makes it a standard engineering requirement rather than an ethical add-on.

6. **Test AI in the deployment context, not just the development context** — performance at a top academic medical center does not predict performance in a rural clinic; evaluate in the target deployment environment.

7. **Use self-supervised learning to leverage unlabeled biological data** — labels are expensive; frame prediction tasks (masked token prediction, contrastive learning) to learn from unlabeled data at scale.

8. **Build AI systems that amplify human intelligence, not replace it** — the goal is to help scientists test more ideas and ask better questions, not to eliminate human judgment from the loop.

9. **Treat LLM text embeddings as biological priors** — gene descriptions, protein annotations, and clinical text encode biological knowledge that can complement or outperform models trained purely on experimental data.

10. **Broaden clinical trial eligibility criteria using real-world data** — many existing criteria are overly restrictive; use EHR data to identify criteria that can be safely relaxed to improve diversity and generalizability.

11. **Concentrate human oversight at high-stakes decision points** — not all AI decisions require human review; focus oversight on final diagnoses, treatment selections, and novel situations where AI uncertainty is highest.

12. **Study AI behavior with model organisms** — use small, controllable models to understand phenomena observed in large, opaque systems; apply the same experimental logic as biological model organism research.
