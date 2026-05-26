# Eugene Myers — Mental Models

Five core mental models that shape how Myers perceives problems and makes decisions.

---

## Mental Model 1 — Biology as String Problems

**Source:** Caltech Heritage interview, ISCB award

Myers's entry into biology was through recognizing that DNA sequences are, at their core, string problems — the same class of problems he was already working on as a computer scientist. This reframing made biology tractable for him and opened up a career.

**The model:** Every biological data type can be reframed as a computational problem:
- DNA sequences → string comparison, approximate matching, assembly
- Protein sequences → string alignment, motif finding
- Microscopy images → 3D reconstruction, object tracking, registration
- Gene expression → matrix factorization, clustering, trajectory inference

**Application:** When encountering a new biological data type, ask: what is the underlying computational problem? What class of algorithms applies? This reframing often reveals that the problem has already been solved in a different domain.

**Key quote:** "Just as a computer scientist looking at it over there, it's like, 'Gee, those biologists have a lot of four-letter strings, DNA strings, or twenty-letter protein strings. I think that's an interesting variation of the problems that we think about.'"

---

## Mental Model 2 — The Heuristic as Theory Approximation

**Source:** Caltech Heritage interview

BLAST was not invented as a practical tool — it was derived from a theoretical result. This is Myers's model for how good heuristics are built: not by trial and error, but by approximating a known optimal solution.

**The model:**
1. Solve the theoretical problem (what is the optimal algorithm?)
2. Identify the bottleneck (what makes the optimal algorithm too slow?)
3. Build a heuristic that approximates the optimal solution while removing the bottleneck
4. Analyze the approximation (what is the error? when does it fail?)

**Why this matters:** A heuristic derived from theory is more robust than one built by trial and error. It has known failure modes, known approximation bounds, and a principled basis for improvement.

**Application:** Before building a heuristic, understand the theoretical optimum. If you don't know what you're approximating, you can't know how good your approximation is.

**Key quote:** "BLAST was basically just a heuristic version of a theoretical result that I was producing, around 1990."

---

## Mental Model 3 — Data as Regenerable Resource

**Source:** "Shifting Ground for Big Data Researchers" profile

Myers's pragmatic model for data management: data is not a precious artifact — it is a regenerable resource. The decision to store or regenerate should be made on economic grounds.

**The model:**
- Data has a regeneration cost (time + money to reproduce)
- Data has a storage cost (infrastructure + maintenance)
- If regeneration cost < storage cost, regenerate on demand
- If regeneration cost > storage cost, store

**The psychological barrier:** Biologists are trained to treat data as precious because historically it was. A clinical sample from a rare patient cannot be regenerated. But a sequencing run from a standard cell line can be regenerated cheaply.

**Application:** Classify your data by regeneration cost. Apply different storage strategies to different classes. Don't let psychological attachment to data drive infrastructure decisions.

**Key quote:** "Generate it, analyze it, throw it away. If you don't like it a week later, then do it again."

---

## Mental Model 4 — Physics as the Missing Layer

**Source:** Caltech Heritage interview

Myers believes that most important biological phenomena cannot be explained without understanding the physical context of molecular processes. Phase transitions, condensation, soft-matter physics — these are not optional extras, they are essential to understanding how cells work.

**The model:**
- Biochemistry describes what molecules do
- Physics describes the context in which they do it
- Many biological phenomena (cell division, AP axis formation, nuclear envelope dissolution) are fundamentally physical processes that happen to involve biochemistry

**Example:** The anterior-posterior axis in worm embryogenesis is controlled by where the sperm enters the egg, which creates a wave in the cytoskeleton — a physical process that affects the stoichiometry of biochemical relationships.

**Application:** When a biological phenomenon seems inexplicable by biochemistry alone, look for the physical mechanism. Ask: what are the phase transitions? What are the condensation events? What is the soft-matter physics?

**Key quote:** "Understanding what a cell does is not just a question of biochemistry. It's a question of biochemistry and physics... the cell very quickly forms complex and solid things and then dissolves them again. If you think about it, when a cell divides, the entire nuclear envelope has to disappear, dissolve, and then you have to reconstitute two nuclear envelopes."

---

## Mental Model 5 — The Genotype-Phenotype Relationship as the Grand Challenge

**Source:** Caltech Heritage interview, MPG portrait

Myers's deepest scientific question: how does the genome create the creature? How do genes determine the shape, the wiring, the behavior of an organism? This is the question that has driven his pivot from sequence analysis to microscopy to connectomics.

**The model:**
- The genome is the program
- Development is the execution of the program
- The phenotype is the output
- Understanding the genotype-phenotype relationship requires understanding the execution, not just the program

**Why this requires new tools:**
- You can't understand execution by reading the source code
- You need to watch the program run — which requires microscopy, imaging, and tracking
- You need to compare execution across species — which requires sequencing everything

**Application:** The most important biological questions are not about sequences — they are about how sequences produce organisms. Build tools that bridge the gap between genotype and phenotype.

**Key quote:** "I want to know how genetics produce the diverse forms that life takes. For example, how do genes determine how the brain of the Drosophila fruit fly is wired and functions?"
