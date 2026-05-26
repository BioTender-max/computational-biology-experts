# Søren Brunak — Conceptual Frameworks

## Framework 1: Disease Trajectory Analysis
**Core insight**: Disease is a temporal sequence of diagnoses, not a static state. By analyzing the order in which diseases manifest over a lifetime, we can identify predictive patterns and intervene earlier.

**Method**:
1. Extract all diagnoses from population-wide EHR data (Danish National Patient Register)
2. Identify statistically significant directional disease associations (A → B more often than expected by chance)
3. Condense millions of individual trajectories into a smaller set of recurrent patterns
4. Visualize as a directed graph of disease transitions

**Scale**: 6.2–7.2 million Danish patients; 14.9 years of registry data; 1,171 significant trajectories identified.

**Application**: Early diagnosis, patient stratification, prevention of adverse outcomes, precision medicine.

**Key tool**: Disease Trajectory Browser (DTB) — interactive tool for exploring 25 years of Danish National Patient Register data.

---

## Framework 2: Disease Systems Biology
**Core insight**: Multi-morbidity is the norm, not the exception. Many genes and pathways play roles in multiple diseases. Understanding disease requires integrating molecular-level systems biology with clinical phenotypic data.

**Method**:
1. Build protein interaction networks from molecular data
2. Map disease-associated genes onto these networks
3. Identify genes and pathways shared across multiple diseases
4. Connect to clinically observed multi-morbidity patterns from EHR data

**Application**: Identifying drug targets relevant across multiple diseases; understanding adverse drug reactions; precision medicine.

---

## Framework 3: Machine Learning for Biological Sequence Analysis
**Core insight**: Biological sequences (proteins, DNA) contain information that can be extracted by machine learning methods trained on known examples.

**SignalP pipeline**:
1. Collect known signal peptides and non-signal peptides
2. Train neural network to distinguish them
3. Predict cleavage sites from sequence alone
4. Apply to new sequences genome-wide

**Philosophy**: In the early data-poor period, machine learning could extract signal from limited data. As data grew, the methods scaled. SignalP has been continuously updated since 1997.

---

## Framework 4: Secure Population-Scale Computing
**Core insight**: Population-wide health data is extraordinarily valuable but extraordinarily sensitive. Secure supercomputing infrastructure is required to handle person-sensitive data at scale.

**Infrastructure**:
- Private cloud solutions designed for population-wide data
- Secure supercomputing infrastructure for person-sensitive data
- Compliance with Danish and EU data protection regulations

**Vision**: Complement classical epidemiology with disease-spectrum-wide analyses in a lifelong perspective.
