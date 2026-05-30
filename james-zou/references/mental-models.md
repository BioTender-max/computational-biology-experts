# Mental Models — James Zou

## 1. AI as Model Organism

Just as biologists use mice to study human disease (because direct human experiments are impossible), Zou uses small, controllable language models to study the behavior of large, opaque systems like GPT-4. When GPT-4 shows behavioral drift, reproduce the phenomenon in a smaller model you control, then use that model to understand the mechanism.

"We've been taking a similar approach with ChatGPT... similar to how people use mice as a model organism for human diseases."

**Application**: When studying the behavior of large, opaque AI systems, identify smaller, controllable model organisms that exhibit the same phenomena. Use these to run controlled experiments and develop mechanistic understanding that can then be applied to the larger system.

---

## 2. The Mad Libs Principle

Self-supervised learning works by asking models to impute missing information from context — missing words, missing amino acids, missing protein domains. If you ask the model to play enough of these "mad libs," it learns the underlying structure and semantics of the data. This principle generalizes across modalities: it works for language, protein sequences, genomic sequences, and medical images.

**Application**: When designing a self-supervised learning task for a new biological modality, ask: what is the natural "missing information" in this data type? What prediction task would force the model to learn the underlying structure? Frame the task as imputation or prediction from context.

---

## 3. The Deployment Gap

There is a systematic gap between AI performance in controlled research settings and AI performance in real-world clinical deployment. This gap arises from distribution shift (new patient populations, new clinical workflows), economic barriers (reimbursement models), and trust deficits (clinician education). Measuring performance at Stanford does not tell you how a model will perform in a rural clinic or another country.

**Application**: When evaluating clinical AI, always ask: in what context was this performance measured? Is that context representative of the target deployment environment? What are the likely sources of distribution shift between the development and deployment contexts?

---

## 4. The Fairness-Robustness Equivalence

Fairness and robustness are not separate concerns — they are the same concern viewed from different angles. A model that performs poorly for minority populations is not robust to demographic distribution shift. A model that is robust to distribution shift will, by definition, perform well across diverse populations.

**Application**: Frame fairness requirements as robustness requirements. Instead of asking "is this model fair?" ask "is this model robust to demographic distribution shift?" This framing makes fairness a standard engineering requirement rather than a separate ethical constraint.

---

## 5. AI Behavioral Drift as a Living System

Large language models are not static artifacts — they are living systems that change over time through feedback, fine-tuning, and safety training. This makes them more like biological organisms than traditional software. Studying their behavioral drift requires the same tools as studying biological systems: longitudinal monitoring, controlled experiments, and model organisms.

**Application**: Treat deployed AI systems as living systems that require ongoing monitoring and maintenance. Define behavioral benchmarks that are evaluated regularly. Build infrastructure for detecting drift and triggering retraining or human review when drift exceeds acceptable thresholds.

---

## 6. The 1% Intervention Rule

In the Virtual Lab, human scientists intervene in only ~1% of the AI agents' operations. This is not a target — it is an empirical observation about where human judgment adds the most value. The implication: human oversight should be concentrated at the highest-stakes decision points, not distributed uniformly across all steps.

**Application**: When designing human-AI collaboration systems, identify the 1% of decisions where human judgment is most valuable (highest stakes, highest uncertainty, most novel situations) and concentrate oversight there. Automate the remaining 99% to maximize efficiency.
