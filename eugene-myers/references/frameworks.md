# Eugene Myers — Frameworks

Four structured frameworks extracted from Caltech Heritage interview, ACGT 101 questions, MPG portrait, and published talks.

---

## Framework 1 — Algorithm-First Biology

**Source:** Caltech Heritage interview, ISCB award, MPG portrait

Myers's approach to computational biology inverts the usual order: instead of starting from a biological question and asking what computation is needed, he starts from algorithmic problems and finds that biology provides the most interesting instances.

**The three-step process:**
1. **Identify the abstract computational problem** — What is the underlying string, graph, or optimization problem?
2. **Solve it theoretically** — What is the optimal algorithm? What are the complexity bounds?
3. **Build the practical heuristic** — What approximation is fast enough to be useful on real data?

**Why this works:**
- Algorithms derived from theory are more robust than ad hoc heuristics
- Theoretical understanding reveals the limits of what's possible
- The same algorithm often applies to multiple biological problems

**Example — BLAST:**
- Abstract problem: approximate string matching with statistical significance
- Theoretical result: neighborhood-based filtering for local alignment
- Practical heuristic: BLAST (Basic Local Alignment Search Tool)

**Example — String Graph:**
- Abstract problem: lossless representation of all valid assemblies from a read set
- Theoretical result: string graph with transitive reduction
- Practical tool: BOA (Berkeley Open Assembler), later DAZZLER

---

## Framework 2 — Pragmatic Data Philosophy

**Source:** "Shifting Ground for Big Data Researchers" profile, Caltech Heritage interview

Myers's framework for managing the data deluge in modern biology. The key insight: not all data is equally valuable to store. The decision to store or regenerate data should be made on economic grounds, not psychological ones.

**The decision matrix:**

| Data Type | Regeneration Cost | Storage Decision |
|-----------|------------------|------------------|
| Clinical samples, rare specimens | Very high | Always store |
| Long-read sequencing runs | Medium | Store raw reads |
| Intermediate analysis files | Low | Regenerate on demand |
| Microscopy images (standard conditions) | Low-medium | Store selectively |

**The key principle:** "Generate it, analyze it, throw it away. If you don't like it a week later, then do it again."

**Why biologists resist this:**
- Psychological attachment to hard-won data
- Fear of losing something irreplaceable
- Cultural norms around data preservation

**Myers's response:** "I think the hardest issue for biologists is psychological. I'm a mathematician, so it's not so hard for me. You have to just run the numbers. It's just a financial decision."

---

## Framework 3 — Cross-Disciplinary Tool-Building

**Source:** Caltech Heritage interview, MPG portrait

Myers's model for how a computational scientist can have maximum impact in biology: not by making biological discoveries, but by building the tools that make discoveries possible.

**The tool-builder's role:**
1. **Identify the bottleneck** — What is the computational step that is limiting biological discovery?
2. **Build the tool** — Solve the algorithmic problem rigorously
3. **Deploy in the lab** — Work closely with biologists to ensure the tool solves the real problem
4. **Maintain and extend** — As data scales and technology changes, update the tool

**The cultural challenge:**
Working across disciplines requires understanding that different fields have different cultures. Computer scientists value theoretical elegance; biologists value experimental validation. A tool that is theoretically optimal but practically unusable will not be adopted.

**Myers's solution:** Spend time in the lab. Go to Celera. Embed yourself in the biological problem until you understand the real constraints.

**The career implication:**
Myers describes himself as a "technologist" — not a computer scientist, not a biologist, but someone who builds the tools that allow biologists to discover things. This is a distinct identity that requires comfort with being neither fully in one camp nor the other.

---

## Framework 4 — Scale-Ahead Design

**Source:** Caltech Heritage interview, ACGT 101 questions

Myers's approach to software design: always build for the data volumes of the next decade, not the current decade.

**The three questions:**
1. **What is the current scale?** — How much data exists today?
2. **What will the scale be in 10 years?** — How fast is data generation growing?
3. **Does my algorithm scale?** — What is the computational complexity? Will it be tractable at 10x, 100x, 1000x the current data?

**Historical examples:**
- 1990: BLAST designed for the databases of the 1990s, but its algorithmic efficiency made it scale to the genomics era
- 2001: Shotgun assembly designed for the human genome, but the string graph formalism scales to any genome
- 2014+: DAZZLER/DALIGNER designed for long-read data before long-read sequencing was mainstream

**The infrastructure gap:**
"We don't have the software infrastructure in place to [compare 100,000 species of genomes]. These are kind of the things that I'm interested in now."

**Implication:** The most valuable computational tools are those that are designed for the scale of data that will exist when the tool matures, not the scale that exists when development begins.
