# Anti-Patterns — Chris Sander

---

## 1. Single-Target Cancer Therapy as a Durable Strategy

**Description**: Designing cancer therapies that target only one molecular
pathway, without accounting for resistance mechanisms.

**Why it fails**: Cancers evolve resistance through secondary mutations within
months of treatment. A single targeted therapy creates selection pressure for
resistance. The correct strategy is combination therapy that blocks multiple
escape pathways simultaneously. "The idea is to use more than one drug, more
than two, and block the exits before the cancer escapes."

---

## 2. Overfitting Predictive Models

**Description**: Building models with more parameters than the data can support.

**Why it fails**: "If you have 10,000 numbers and only 2,000 experiments, you
might as well forget it." Overfitted models memorize training data and fail to
generalize. The art of computational biology is finding the minimal model that
captures the main essence of the system.

---

## 3. Predicting Structure from Local Sequence Alone

**Description**: Using only the local sequence context (5 residues or fewer)
to predict secondary structure or conformation.

**Why it fails**: Identical pentapeptides can have completely different
conformations depending on their sequence context. Cooperativity of length six
or longer must be taken into account. Methods that ignore sequence context
systematically fail at secondary structure prediction.

---

## 4. Ignoring Evolutionary Information in Structure Prediction

**Description**: Using single-sequence methods when multiple sequence alignments
are available.

**Why it fails**: Including multiple sequence alignments as input increases
prediction accuracy by 6–8 percentage points over single-sequence methods.
Evolutionary profiles encode structural constraints that no single sequence
can reveal. Ignoring them is leaving the most powerful signal on the table.

---

## 5. Building Proprietary Bioinformatics Tools

**Description**: Developing bioinformatics tools that are not freely available
to the research community.

**Why it fails**: cBioPortal and Pathway Commons became community standards
precisely because they were open. Proprietary tools create silos, slow adoption,
and are eventually outcompeted by open alternatives. The community accelerates
faster than any single lab.

---

## 6. Observing Without Perturbing

**Description**: Trying to understand complex biological systems through
observational data alone, without systematic perturbation experiments.

**Why it fails**: Correlation in observational data does not reveal causal
structure. Systematic perturbation — with rich readouts — is required to build
predictive models of network behavior. Observation tells you what; perturbation
tells you why.
