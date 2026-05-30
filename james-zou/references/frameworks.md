# Frameworks — James Zou

## 1. The Virtual Lab — Autonomous Multi-Agent Scientific Discovery

A framework for conducting scientific research using autonomous AI agents with minimal human oversight.

**Architecture**:
- **AI Principal Investigator (PI)**: Oversees the project, assigns tasks, and coordinates the team
- **Specialist Researcher Agents**: Each specializes in a different discipline (protein design, literature review, data analysis, etc.)
- **Scientific Critic Agent**: Reviews the group's work, identifies weak assumptions and logical gaps
- **Agent School**: A training environment where agents read papers, explore data repositories, and quiz themselves before joining the lab

**Workflow**:
1. Human scientist poses a scientific challenge (e.g., "Design a nanobody that binds to a new COVID variant")
2. AI PI recruits specialist sub-agents and conducts concurrent lab meetings
3. Agents cite literature, propose hypotheses, debate methods, and integrate results
4. Human scientists intervene in ~1% of operations
5. Validated outputs are synthesized and tested in the wet lab

**Demonstrated result**: AI-designed nanobodies outperformed previous human-designed nanobodies as binders to new COVID variants.

**Key insight**: AI agents can replicate the creative and collaborative process of scientific teamwork at machine speed — hundreds of discussions in the time a human team has one meeting.

**Source**: Stanford Cancer Institute (2026); Stanford HAI (2026); Zou & Topol (2025), *Lancet*.

---

## 2. GenePT — Literature-Grounded Foundation Models for Single-Cell Biology

A framework for building foundation models for genomics by leveraging language model embeddings of gene descriptions.

**Insight**: Most single-cell foundation models learn from statistical correlations across millions of cells. But the biological knowledge encoded in scientific literature — gene function, pathway membership, disease associations — is not captured by expression data alone.

**Method**:
1. Use NCBI text descriptions of individual genes
2. Generate embeddings using GPT-3.5
3. Create single-cell embeddings by averaging gene embeddings weighted by expression level, or by creating sentence embeddings ordered by expression

**Result**: GenePT achieves comparable or better performance than Geneformer on cell type classification and other downstream tasks, without requiring dataset curation or additional pretraining.

**Broader principle**: Text embeddings of biological entities can serve as powerful priors that complement or even outperform models trained purely on experimental data.

**Source**: Chen & Zou (2023), *bioRxiv*; Ground Truths podcast (2023).

---

## 3. Trial Pathfinder — AI-Driven Clinical Trial Eligibility Optimization

A framework for using real-world data to evaluate and broaden clinical trial eligibility criteria.

**Problem**: Clinical trial eligibility criteria are often overly restrictive, excluding women, minorities, and older patients — reducing both enrollment and generalizability of results.

**Method**:
1. Use real-world electronic health record data to simulate trial enrollment under different eligibility criteria
2. Evaluate the impact of relaxing specific criteria on enrollment diversity and adverse event rates
3. Identify criteria that can be safely broadened without increasing safety risks

**Key finding**: Many existing eligibility criteria can be substantially relaxed while maintaining safety, enabling much more diverse and larger patient populations to enroll.

**Impact**: Growing recognition from FDA, EMA, and pharmaceutical companies that clinical trials are often overly narrow; Trial Pathfinder provides a computational framework for evidence-based criteria design.

**Source**: EMJ interview (2026).

---

## 4. Fairness-Aware AI Development Pipeline

A systematic framework for identifying and mitigating bias throughout the AI model lifecycle.

**Stage 1 — Outcome Design**: Ensure that the outcome being predicted is meaningful and equitable across populations. Biased outcome definitions propagate through the entire pipeline.

**Stage 2 — Data Collection**: Audit training data for demographic representation. Non-representative samples produce models that generalize poorly to underrepresented groups.

**Stage 3 — Algorithm Development**: Use techniques such as:
- Disentanglement: separating ancestry from phenotype-relevant information in polygenic risk models
- Federated learning: training across institutions without centralizing sensitive data
- Adversarial debiasing: training models to be invariant to protected attributes

**Stage 4 — Evaluation**: Stratify performance metrics across subpopulations. Headline accuracy metrics can mask large disparities in performance across demographic groups.

**Stage 5 — Deployment and Monitoring**: Continuously monitor model behavior in deployment. Require vendors to provide transparent statistics on training population demographics. Implement post-market surveillance analogous to medical device regulation.

**Key principle**: Bias and fairness are components of robustness. A model that fails for minority populations is not robust.

**Source**: Zou & Schiebinger (2018), *Nature*; Zou & Schiebinger (2021), *EBioMedicine*; EMJ interview (2026).

---

## 5. Multimodal Foundation Models for Clinical AI

A framework for building AI systems that integrate multiple data modalities for clinical decision support.

**Modalities**:
- Pathology images (digital slides)
- Radiology images (CT, MRI, ultrasound video)
- Genomic sequences (DNA, RNA, single-cell profiles)
- Clinical text (EHR notes, pathology reports)
- Physiological waveforms (ECG, sleep recordings)

**Architecture**: Transformer-based models that process each modality through modality-specific encoders, then integrate representations through cross-modal attention.

**Key insight**: Transformers, originally developed for text, have proven surprisingly effective for imaging and waveform data. Visual transformers outperform convolutional neural networks on many medical imaging tasks.

**Application examples**:
- Visual-language model trained on 200,000+ pathology tweets (images + expert discussion text)
- Cardiovascular disease diagnosis from ultrasound videos (FDA-cleared)
- 130+ disease prediction from one night of sleep recording

**Frontier**: Consumer-accessible wearables as a source of multimodal health data — democratizing health monitoring beyond clinical settings.

**Source**: Ground Truths podcast (2023); EMJ interview (2026); Stanford HAI (2026).
