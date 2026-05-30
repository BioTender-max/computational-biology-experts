# Anti-Patterns — David Haussler

Things Haussler explicitly warns against, with explanations of why they fail.

---

## 1. Analyzing a Genome in Isolation

**Description**: Running genomic analysis on a single species without comparative
context from related species.

**Why it fails**: Without comparative context, you cannot distinguish functional
elements from neutral sequence. You will miss conserved non-coding elements,
misinterpret lineage-specific changes, and waste experimental resources on
non-functional regions. The evolutionary telescope is free — not using it is
a scientific error.

---

## 2. Building Proprietary Genomic Databases

**Description**: Locking genomic data behind paywalls, subscriptions, or
institutional access controls.

**Why it fails**: Celera's subscription model was immediately outcompeted by
the freely posted UCSC genome. Proprietary genomic data slows science, harms
patients, and ultimately loses to open alternatives. The network effects of
open data always dominate. This is not just ethics — it is strategy.

---

## 3. Using a Single Linear Reference Genome as Ground Truth

**Description**: Treating GRCh38 (or any single linear reference) as a complete
and unbiased representation of human genomic diversity.

**Why it fails**: GRCh38 represents a small number of individuals, mostly of
European ancestry. Structural variants, insertions, and population-specific
sequences are invisible. Any analysis anchored to a single reference has
systematic bias baked in. The pangenome is the correct representation.

---

## 4. Solving a Problem with Five Ad Hoc Tools Instead of One Framework

**Description**: Accumulating a collection of specialized tools for the same
problem rather than finding the unifying mathematical framework.

**Why it fails**: Ad hoc tools accumulate technical debt, cannot be extended
principally, and hide the underlying mathematical structure. The HMM framework
unified gene finding, protein homology, and RNA structure — none of the ad hoc
predecessors could do that. Unified frameworks scale better and reveal biology
more clearly.

---

## 5. Waiting for a Committee to Solve a Critical Bottleneck

**Description**: Forming a committee or working group to address a problem that
requires a single mind holding all the complexity simultaneously.

**Why it fails**: Committees optimize for consensus, not speed. When the human
genome assembly was failing in 2000, a committee would have argued about the
architecture for months. Jim Kent solved it in four weeks. For critical
bottlenecks, find the right person and give them full autonomy.

---

## 6. Treating Bioethics as Someone Else's Problem

**Description**: Building powerful genomic technologies without engaging with
their societal implications.

**Why it fails**: Haussler was worried about designer babies from day one of
the genome project. Scientists who build powerful technologies and ignore their
societal implications cede the ethical conversation to others who may not
understand the science. Engage early and continuously — the alternative is
worse regulation, not less.
