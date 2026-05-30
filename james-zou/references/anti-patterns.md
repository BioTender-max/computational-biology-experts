# Anti-Patterns — James Zou

## 1. Optimizing for Headline Metrics

**The mistake**: Reporting a single accuracy number on a held-out test set, without stratifying by subpopulation or evaluating in the target deployment context.

**Why it fails**: Headline metrics are context-dependent and can mask large disparities. A model with 95% overall accuracy may have 70% accuracy for a minority subgroup. Performance at Stanford does not predict performance in a rural clinic or another country.

**The fix**: Always stratify performance metrics by demographic group, clinical site, and data source. Report confidence intervals. Evaluate in the target deployment context, not just the development context.

---

## 2. Static Model Deployment

**The mistake**: Deploying an AI model once and assuming it will perform consistently over time.

**Why it fails**: LLMs change through fine-tuning and safety training; clinical AI models face distribution shift as patient populations and clinical workflows evolve. Zou's lab showed that GPT-4's chain-of-thought reasoning ability degraded substantially over time, even as safety improved. Static deployment without continuous monitoring is a patient safety risk.

**The fix**: Implement continuous behavioral monitoring for deployed AI systems. Define key performance indicators evaluated regularly. Build infrastructure for detecting distribution shift and model drift. Treat AI deployment as an ongoing process, not a one-time event.

---

## 3. Treating Fairness as a Post-Hoc Fix

**The mistake**: Attempting to de-bias a model after it has been trained on non-representative data.

**Why it fails**: Post-hoc debiasing is much harder than collecting diverse data from the start. Bias embedded in training data propagates through the entire model and is difficult to remove without retraining. Fairness must be integrated into outcome design, data collection, and algorithm development.

**The fix**: Audit training data for demographic representation before model development begins. Collect data from diverse populations, clinical sites, and geographic regions. Integrate fairness evaluation into every stage of the development pipeline.

---

## 4. Assuming Research Performance Equals Clinical Performance

**The mistake**: Assuming that a model achieving state-of-the-art performance on a benchmark dataset will perform similarly in clinical deployment.

**Why it fails**: The deployment gap is systematic and predictable. Distribution shift (new patient populations, different clinical workflows, different data quality), economic barriers, and trust deficits all contribute to performance degradation in deployment. This gap must be explicitly addressed, not assumed away.

**The fix**: Evaluate AI systems in the target deployment context before deployment. Conduct prospective clinical studies. Build relationships with clinical partners who can provide real-world deployment contexts for evaluation.

---

## 5. Black-Box Clinical AI

**The mistake**: Deploying AI systems in clinical settings without interpretable explanations for their predictions.

**Why it fails**: Clinicians cannot trust predictions they cannot understand. Black-box models make it impossible to identify failure modes, detect when a model is making errors for the wrong reasons, or explain decisions to patients. Interpretability is a prerequisite for safe clinical deployment.

**The fix**: Design models with interpretable features from the start. Use attention visualization, feature attribution, and other interpretability methods. Ensure every clinical prediction is traceable to specific input features and evidence.

---

## 6. Ignoring the Economics of Deployment

**The mistake**: Building a technically excellent AI system without a viable reimbursement model or economic pathway to deployment.

**Why it fails**: Over 1,000 AI medical devices have FDA clearance, but only a handful are widely deployed. The bottleneck is not algorithmic performance — it is economics. Without a sustainable financial model, even excellent AI systems will not reach patients.

**The fix**: Engage with payers, health systems, and regulators early in the development process. Understand the reimbursement landscape. Design studies that generate the evidence needed to support reimbursement decisions. Build economic models alongside technical models.
