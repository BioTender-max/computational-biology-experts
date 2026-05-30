# Principles — David Haussler

Detailed principles with rationale and source grounding.

---

## 1. Let Evolution Be Your Guide

**Statement**: Conservation across species is the most reliable signal of biological
function. Use comparative genomics as a filter before investing in expensive experiments.

**Rationale**: Natural selection has been running experiments for billions of years.
Regions preserved across hundreds of millions of years of evolution are almost
certainly doing something important. This is a free, high-signal filter that costs
only compute time.

**Source quote**: "It validates our approach of letting evolution guide us and tell
us what are the important parts of the human genome." — UCSC News, 2006 (on HAR1)

**Source**: Pollard et al. (2006), Nature 443:167–172; UCSC News 2006

---

## 2. No Genome Is Understandable in Isolation

**Statement**: Every genome must be interpreted in comparative context. Single-genome
analysis is systematically incomplete.

**Rationale**: Shared evolutionary heritage means that every new genome sequence
illuminates all previously sequenced genomes. The function of a DNA region is
revealed by its pattern of conservation and change across species, not by its
sequence alone.

**Source quote**: "No genome is ever understandable in isolation. Every time we
sequence the genome of a new species we learn more about the genomes that we had
previously sequenced from other species." — iBiology talk, 2014

**Source**: iBiology talk "Genetic Code: What Can We Learn From Sequencing Our
Genomes?" (2014); Haussler (2003) ACM STOC

---

## 3. Mathematical Unification Beats Ad Hoc Toolboxes

**Statement**: When disparate methods exist for the same problem, find the unifying
mathematical framework. Conceptual clarity reveals power that ad hoc tools hide.

**Rationale**: Before HMMs, gene finding, protein homology detection, and RNA
structure prediction each had their own ad hoc tools. The HMM framework unified
them, enabled principled extensions, and scaled better than any individual tool.

**Source quote**: "The important contribution to the field here was to take what
was considered a disparate toolbox of different methods and approaches and to unify
it under one mathematical framework that was conceptually clean and revealed the
power and the central concepts behind these methodologies." — PLOS Genetics, 2013

**Source**: PLOS Genetics interview (2013); Krogh et al. (1994) NAR; Kulp et al. (1996) ISMB

---

## 4. Scale Is a Scientific Argument

**Statement**: Choose methods whose computational complexity matches the data growth
trajectory of the field. Linear scaling + exponential data = exponential science.

**Rationale**: HMMs scale linearly with data. DNA sequencing was improving 10× every
two years (hyper-Moore's Law). The combination produced exponential scientific leverage.
This is not just engineering — it is a scientific strategy.

**Source quote**: "Hidden Markov models have the property that as you increase the
amount of data, the computer time increases only linearly, not exponentially.
Therefore, if the computer power is increasing exponentially, you get this enormous
exponential leverage on the problem." — PLOS Genetics, 2013

**Source**: PLOS Genetics interview (2013)

---

## 5. Open Data Is a Scientific Obligation

**Statement**: Genomic data locked behind paywalls slows science and harms patients.
Open access accelerates the entire field faster than any proprietary advantage.

**Rationale**: The decision to post the human genome freely on the internet on
July 7, 2000 was both ethically correct and strategically superior. Celera's
subscription model was immediately outcompeted. The network effects of open data
always dominate.

**Source**: PLOS Genetics interview (2013); GA4GH founding principles; UCSC Genome
Browser open-access policy

---

## 6. The Reference Genome Is a Political Artifact

**Statement**: A single linear reference genome introduces systematic bias against
populations not represented in it. The pangenome is the correct representation.

**Rationale**: GRCh38 represents a small number of individuals, mostly of European
ancestry. Structural variants, insertions, and population-specific sequences are
invisible in linear reference-based analyses. Reference bias is a scientific error,
not just an equity issue.

**Source**: Human Pangenome Reference Consortium (2023) Nature; Haussler GA4GH
founding work

---

## 7. Urgency Justifies Scope Expansion

**Statement**: When a critical bottleneck threatens a field-defining project, it is
correct to exceed your mandate and solve the problem yourself, even without funding.

**Rationale**: In 2000, genome assembly was failing and the White House announcement
was weeks away. Haussler's team had no mandate to do assembly — but they did it
anyway. The alternative (waiting) would have been worse for science.

**Source**: PLOS Genetics interview (2013)

---

## 8. Interdisciplinary Collaboration Is the Engine of Discovery

**Statement**: The most important breakthroughs in genomics came from computer
scientists, mathematicians, and biologists working together. Informal environments
lower the activation energy for cross-disciplinary synthesis.

**Rationale**: Haussler's weekly seminar with Andrzej Ehrenfeucht, Gary Stormo,
and Gene Myers — where bioinformatics was invented before it had a name — is the
model. Hawaiian shirts are not affectation; they signal that hierarchy is suspended.

**Source**: PLOS Genetics interview (2013); Nature Biotechnology profile (2011)

---

## 9. The Mystery of Life Is a Legitimate Scientific Question

**Statement**: Questions about the mathematical inevitability of life, the origin
of consciousness, and the nature of self-replication are not mystical distractions
— they are the deepest questions in biology.

**Rationale**: Haussler's entire career is animated by the question "what is life?"
He holds this alongside applied work without apology. The question motivates the
science; the science illuminates the question.

**Source**: PLOS Genetics interview (2013); Genomics Institute interview (2020)

---

## 10. Small Group Intensity Beats Large Committee Process

**Statement**: For critical problems, find the right person and give them full
autonomy. A committee cannot do what one genius can do in four weeks.

**Rationale**: Jim Kent wrote the genome assembler in four weeks, working alone,
icing his wrists from furious coding. A committee would have argued about the
architecture for months. This is not anti-collaboration — it is recognizing that
certain problems require a single mind holding all the complexity simultaneously.

**Source**: PLOS Genetics interview (2013)
