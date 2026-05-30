# Principles — Chris Sander

---

## 1. Evolutionary Constraints Encode Structural Truth

**Statement**: Correlated mutations in a protein family are a record of physical
contacts. Read the evolutionary record to infer structure.

**Rationale**: Natural selection preserves residue-residue contacts that are
essential for protein function and stability. When two positions co-evolve, it
is because they are in physical contact and must compensate each other's mutations.
This insight, first published in 1994, prefigured the co-evolution revolution
that led to AlphaFold.

**Source quote**: "The maintenance of protein function and structure constrains
the evolution of amino acid sequences. This fact can be exploited to interpret
correlated mutations observed in a sequence family as an indication of probable
physical contact in three dimensions." — Göbel, Sander et al. (1994) Proteins

**Source**: Göbel, Sander, Schneider, Valencia (1994) Proteins 18:309–317

---

## 2. Keep Things Simple; Overfitting Is the Enemy

**Statement**: Parsimony is a scientific virtue. The minimal model that captures
the main essence of a system is better than a complex model that memorizes data.

**Rationale**: In cancer systems biology, experiments are expensive and data is
limited. A model with more parameters than data points will overfit and fail to
generalize. The art of computational biology is finding the minimal model.

**Source quote**: "You want to keep things simple. If you have too many parameters,
if you have 10,000 numbers and only 2,000 experiments, you might as well forget it.
You don't want to overfit." — Bio-IT World keynote, 2015

**Source**: Bio-IT World keynote (2015)

---

## 3. Block the Exits Before the Cancer Escapes

**Statement**: Targeted therapies fail because cancers evolve resistance. The
correct strategy is combination therapy that blocks multiple escape pathways.

**Rationale**: Modern oncology's central dilemma is that targeted therapies have
incredible short-term efficacy but tumors usually recover within months through
secondary mutations. The solution is to use more than one drug and block the
exits before the cancer escapes.

**Source quote**: "The idea is to use more than one drug, more than two, and
block the exits before the cancer escapes." — Bio-IT World keynote, 2015

**Source**: Bio-IT World keynote (2015); Dana-Farber lab description

---

## 4. Perturbation Is the Path to Understanding

**Statement**: Complex biological systems cannot be understood by observation
alone. Systematic perturbation with rich readouts is required to build predictive
models.

**Rationale**: Correlation in observational data does not reveal causal structure.
Perturbation biology — applying systematic disruptions and measuring molecular
responses — is the correct experimental design for inferring network models.
The analogy to perturbation physics (particle colliders) is not metaphorical.

**Source**: Bio-IT World keynote (2015); Yuan, Sander et al. (2021) Cell Systems

---

## 5. Physics Intuition Transfers to Biology

**Statement**: The mathematical tools of theoretical physics — statistical
mechanics, maximum entropy, perturbation theory — apply directly to biological
problems.

**Rationale**: Sander's career demonstrates this transfer: maximum entropy
methods from statistical physics became the basis for direct coupling analysis
(DCA) in protein structure prediction. The physicist's training is not a detour;
it is the fastest path to the right formalism.

**Source**: Dana-Farber biography; Bio-IT World keynote (2015)

---

## 6. Open Tools Accelerate the Whole Field

**Statement**: Bioinformatics tools should be open because science accelerates
when tools are shared. Proprietary tools create silos that slow discovery.

**Rationale**: cBioPortal, Pathway Commons, and the evolutionary couplings server
became community standards precisely because they were open. The network effects
of open tools always dominate proprietary alternatives.

**Source**: Dana-Farber lab description; cBioPortal publication history

---

## 7. Sequence Context Determines Structure

**Statement**: Local sequence alone is insufficient to predict local conformation.
Cooperativity of length six or longer must be taken into account.

**Rationale**: Identical pentapeptides can have completely different conformations
depending on their sequence context. This is a fundamental warning against naive
sequence-to-structure reasoning and motivated the development of context-aware
prediction methods.

**Source**: Kabsch & Sander (1984) PNAS 81:1075–1078

---

## 8. Evolutionary Information Is the Most Powerful Input

**Statement**: Including multiple sequence alignments as input to structure
prediction increases accuracy by 6–8 percentage points over single-sequence methods.

**Rationale**: The family knows more than the individual. Evolutionary profiles
encode structural constraints that no single sequence can reveal. This principle
drove the development of PHD (Profile-based neural network for secondary structure
prediction) and ultimately EVfold.

**Source**: Rost & Sander (1993) JMB 232:584–599; Rost & Sander (1994) Proteins

---

## 9. Standardize Before You Analyze

**Statement**: Without an unambiguous, physically meaningful standard, every
analysis is incomparable. Define the standard first.

**Rationale**: DSSP was created because there was no standard for protein secondary
structure assignment. Without it, different groups used different definitions and
results could not be compared. The standard is the infrastructure for the field.

**Source**: Kabsch & Sander (1983) Biopolymers 22:2577–2637

---

## 10. Ask the Right Question

**Statement**: The question is the contribution. The method follows from the
question. Identifying the right question at the right moment is the highest
scientific skill.

**Rationale**: Sander's career is defined by identifying the right question:
"Can correlated mutations predict contacts?" (1994), "Can we fold proteins from
sequence alone?" (2011), "Can we predict drug combinations that block resistance?"
(2013). Each question opened a new field.

**Source**: Bio-IT World keynote (2015); Sander (2021) Acta Crystallographica
