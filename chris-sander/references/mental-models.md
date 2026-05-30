# Mental Models — Chris Sander

---

## 1. The Physicist's Lens on Biology

**Description**: Biology is a physical system subject to quantitative constraints.
The tools of theoretical physics — statistical mechanics, maximum entropy,
perturbation theory — apply directly.

**Example**: Maximum entropy methods from statistical physics became the basis
for direct coupling analysis (DCA), which extracts direct residue-residue
couplings from multiple sequence alignments. The same mathematical framework
used to model spin glasses was used to predict protein contacts.

**Application**: When a biological problem seems intractable, ask: what are the
physical constraints? What is the statistical mechanical formulation? The physics
formulation often reveals the solution.

---

## 2. The Escape Pathway Map

**Description**: Cancer is not a static target — it is an evolving system that
finds escape routes around any single blockade. The therapeutic goal is to block
all exits simultaneously.

**Example**: Gleevec (imatinib) was spectacularly effective against BCR-ABL
leukemia, but resistance developed within months through secondary mutations.
The escape pathway map for BCR-ABL includes dozens of resistance mutations;
combination therapies that block multiple pathways are more durable.

**Application**: Before designing a therapy, map all known resistance mechanisms.
Design combinations that block the primary target and all escape routes. Single-
target therapy is playing whack-a-mole with an evolving adversary.

---

## 3. The Evolutionary Record as Structural Data

**Description**: A multiple sequence alignment is a record of millions of years
of evolutionary experiments. Every correlated mutation is a data point about
physical contact.

**Example**: In 1994, Sander's group showed that correlated mutations in protein
families predict residue-residue contacts with accuracy 1.4–5.1× better than
random. This insight, extended by maximum entropy methods, became the basis for
EVfold and ultimately influenced AlphaFold's co-evolution features.

**Application**: Before running structural experiments, mine the evolutionary
record. Build a multiple sequence alignment, compute correlated mutations, use
them as structural constraints. The evolutionary record is free and powerful.

---

## 4. The Multifocal Glasses of Systems Biology

**Description**: The single-gene view of cancer is myopic. Systems biology
provides multifocal glasses that see the whole cell simultaneously.

**Example**: "Instead of looking in one place only, we observe the whole cancer
cell and study its properties comprehensively. This is called systems biology.
It is like wearing a pair of multifocal glasses." — Sander, Einstein Foundation.
Single-gene targeted therapy fails because it ignores the rest of the network.

**Application**: When analyzing cancer, don't focus on a single gene or pathway.
Profile the whole molecular landscape. Build network models. The cancer's
behavior emerges from the network, not from any single node.

---

## 5. The Perturbation Collider

**Description**: Just as particle physicists use colliders to probe the structure
of matter, biologists can probe cellular networks by perturbing them with drugs
and measuring molecular responses.

**Example**: Sander's perturbation biology framework applies thousands of drug
perturbations to cancer cells and measures the molecular responses. The data is
used to infer a network model — exactly as particle physicists use collision data
to infer the structure of matter.

**Application**: Design experiments as perturbation experiments, not observation
experiments. Apply systematic disruptions. Measure richly. Use the responses to
build a model. The model is the understanding.

---

## 6. The Sequence-Structure Gap

**Description**: The gap between the number of known protein sequences and known
protein structures is not a temporary inconvenience — it is a fundamental challenge
that requires computational solutions.

**Example**: In 1993, ~30,000 protein sequences were known but only ~1,000
structures. By 2024, hundreds of millions of sequences are known but only ~200,000
experimental structures. The gap has widened by orders of magnitude. AlphaFold
addressed this gap computationally.

**Application**: When designing a research program, ask: where is the gap? The
gap between what we can measure and what we can understand is where computational
biology lives. The gap is the field.
