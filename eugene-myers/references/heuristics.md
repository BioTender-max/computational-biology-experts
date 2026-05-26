# Eugene Myers — Heuristics

18 actionable heuristics across 4 categories, distilled from Caltech Heritage interview, ACGT 101 questions, MPG portrait, and ISCB award.

---

## Category A — Algorithm Design

**H1. Derive Heuristics from Theory**
Before building a practical tool, solve the theoretical problem. Understand the optimal algorithm, identify its bottleneck, and build a heuristic that approximates it. BLAST was a heuristic version of a theoretical result — not an ad hoc invention.

**H2. Design for the Worst Case, Optimize for the Common Case**
Understand the theoretical complexity of your algorithm. Design it to be correct in the worst case, then optimize for the common case that actually occurs in practice.

**H3. Use Filters to Eliminate Non-Candidates**
BLAST's key insight: use a fast filter (k-mer matching) to eliminate most of the search space before applying the expensive exact algorithm. A filter that is fast and specific can improve the speed of an exact algorithm by orders of magnitude.

**H4. Build End-to-End Systems**
Avoid pipelines where each stage is optimized independently. End-to-end systems allow the algorithm to discover representations that serve the final objective, not intermediate proxies.

**H5. Think About Transitive Reduction**
In graph-based assembly, many edges are redundant — they can be inferred from other edges. Transitive reduction removes these redundant edges, simplifying the graph without losing information. Apply this principle broadly: look for redundancy in your data structures.

---

## Category B — Data and Scale

**H6. Classify Data by Regeneration Cost**
Before deciding whether to store data, estimate the cost of regenerating it. If regeneration is cheap, don't store it. Apply different storage strategies to different data classes.

**H7. Design for 10x the Current Scale**
When building software, design for data volumes that are 10x larger than what currently exists. Scalability is not an optimization — it is a design requirement.

**H8. Prefer Long Reads When Available**
Short reads produce "truly miserable reconstructions of novel genomes." Long reads are fundamentally better for assembly because they span more repeats. When the technology is available, use it.

**H9. Sequence Everything**
The genotype-phenotype relationship is best understood by comparing many species, not by exhaustively studying one. "I think we're going to learn more about the genotype/phenotype relationship from studying all of the genotypes and phenotypes in nature than we are by studying human genomes and phenotypes to exhaustion."

**H10. Build Infrastructure Before You Need It**
The software infrastructure for comparing 100,000 species of genomes doesn't exist yet. Build it before the data arrives, not after.

---

## Category C — Career and Research

**H11. Learn Mathematics and Programming Early**
"Learn mathematics and programming now while your mind is young and supple, you can acquire a large corpus of knowledge about biological processes later." The reverse is much harder.

**H12. Stay in the Code**
Write code yourself, even as a leader. The moment you stop doing the work, you lose the ability to make good decisions about it. Myers writes code first thing every morning.

**H13. Keep Groups Small**
Myers's ideal group size is 12. Small groups allow the leader to know every person's work, maintain quality, and avoid the overhead of large organizations.

**H14. Choose Problems with Unsolved Algorithmic Core**
"There are still cool unsolved problems to explore despite the fact that some core aspects of the field, now in its middle-age in my view, are 'overworked'." Seek problems where the algorithmic challenge is still open.

**H15. Pivot When a New Modality Opens**
When a new instrument or data type creates new algorithmic problems, pivot. Myers pivoted from sequence analysis to microscopy after seeing a cell division video. New modalities create new opportunities for algorithmicists.

---

## Category D — Interdisciplinary Work

**H16. Understand the Culture of the Other Field**
Before collaborating across disciplines, invest time in understanding the other field's culture. What counts as a result? What counts as rigor? What is the standard of proof? Cultural fluency is as important as technical fluency.

**H17. Embed Yourself in the Real Problem**
Don't design algorithms for idealized data. Spend time with the actual instruments, the actual data, the actual constraints. Myers's algorithms improved dramatically when he went to Celera and had to deal with real sequencing machines.

**H18. Choose Model Organisms for Experimental Tractability**
The right model organism is the one that allows you to do experiments quickly and cheaply. "Why are you doing that in mice, where it takes a year to breed a mouse? You can do the same thing in a fly and it's five days."
