# Eugene Myers — Anti-Patterns

Six failure modes that Myers explicitly warns against or has observed in the field.

---

## Anti-Pattern 1 — Stamp-Collecting Omics

**Description:** Generating large lists of molecular parts (genes, proteins, metabolites) without mechanistic insight. Myers calls this "stamp collecting" — accumulating data without understanding what it means.

**Myers's diagnosis:** "I'm really bored with networks and -omics. Stamp collecting large parts lists seems to have become the norm despite the fact that it rarely leads to much mechanistic insight."

**The trap:** Confusing data generation with scientific progress. A list of 10,000 differentially expressed genes is not an explanation — it is a starting point for an explanation.

**Correction:** Ask what mechanism the data reveals. If the data doesn't constrain a mechanistic model, it is not yet science — it is inventory.

---

## Anti-Pattern 2 — Short-Read Myopia

**Description:** Relying on short-read sequencing for applications that require long reads, particularly de novo genome assembly of novel organisms.

**Myers's diagnosis:** "I was disgusted with the short-read DNA sequencers that, while cheap, produce truly miserable reconstructions of novel genomes. Good only for resequencing and digital gene expression/transcriptomics."

**The trap:** Choosing the cheapest technology rather than the right technology. Short reads are excellent for resequencing and RNA-seq, but they cannot span repetitive regions and produce fragmented assemblies of novel genomes.

**Correction:** Match the sequencing technology to the question. For de novo assembly of novel genomes, use long reads. For resequencing and expression analysis, short reads are appropriate.

---

## Anti-Pattern 3 — Data Hoarding

**Description:** Storing all data indefinitely, regardless of regeneration cost, out of psychological attachment or cultural norms.

**Myers's diagnosis:** "I think the hardest issue for biologists is psychological. I'm a mathematician, so it's not so hard for me. You have to just run the numbers. It's just a financial decision."

**The trap:** Treating all data as equally precious. This leads to massive storage costs for data that could be cheaply regenerated, and diverts resources from actual research.

**Correction:** Classify data by regeneration cost. Store only what is expensive to regenerate. For cheap-to-regenerate data, store the protocol and parameters, not the data itself.

---

## Anti-Pattern 4 — Ignoring Physics

**Description:** Trying to explain biological phenomena using only biochemistry, without considering the physical context (phase transitions, condensation, soft-matter physics).

**Myers's diagnosis:** "Without an understanding of spatial organization and soft-matter physics, most important biological phenomenon cannot be explained."

**The trap:** Biochemistry is necessary but not sufficient for understanding cellular processes. Many phenomena — cell division, organelle formation, AP axis establishment — are fundamentally physical processes that happen to involve biochemistry.

**Correction:** When a biological phenomenon seems inexplicable by biochemistry alone, look for the physical mechanism. Recruit physicists to your team. Read the soft-matter physics literature.

---

## Anti-Pattern 5 — Staying in One Discipline

**Description:** Remaining within the boundaries of a single discipline when the most interesting problems are at the intersections.

**Myers's diagnosis:** "A lot of people talk about working across disciplines, but people are either naïve about the cultural differences, and the fact that they have to be attuned to the cultural differences in the sciences."

**The trap:** Interdisciplinary work is harder than it looks. It requires not just technical knowledge of multiple fields, but cultural fluency — understanding how different fields define rigor, evidence, and success.

**Correction:** Invest in cultural fluency, not just technical knowledge. Spend time in the other field's seminars, read their papers, understand their standards. Then build tools that speak both languages.

---

## Anti-Pattern 6 — Overworked Problems

**Description:** Continuing to work on problems that have been "overworked" — where the core algorithmic challenges have been solved and further work produces diminishing returns.

**Myers's diagnosis:** "There are still cool unsolved problems to explore despite the fact that some core aspects of the field, now in its middle-age in my view, are 'overworked'."

**The trap:** Staying in a comfortable, well-established area because it is safe and publishable, rather than moving to harder, less-explored problems.

**Correction:** Regularly audit your research agenda. Ask: is this problem still algorithmically interesting? Are there still fundamental open questions? If not, look for the next frontier.
