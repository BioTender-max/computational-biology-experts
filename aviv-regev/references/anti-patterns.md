# Aviv Regev — Anti-Patterns

Seven failure modes that Regev explicitly warns against or has observed in the field.

---

## Anti-Pattern 1 — Bulk Averaging (The Smoothie Problem)

**Description:** Using bulk RNA sequencing for questions that require single-cell resolution. Bulk measurements average across millions of cells, obscuring the heterogeneity that drives biology.

**Regev's diagnosis:** "Previous techniques required blending many different cells together to have enough material to study, making it challenging to distinguish a particular type of cell, more like trying to pick out the blueberries from a smoothie made from many other types of fruit."

**The trap:** Bulk measurements are cheaper and easier than single-cell measurements. But for questions involving cell type heterogeneity, rare cell types, or cell state transitions, bulk measurements are not just less informative — they are actively misleading.

**Correction:** For any question involving complex tissues, use single-cell resolution. The cost of single-cell RNA-seq has dropped to pennies per cell — the cost argument no longer holds.

---

## Anti-Pattern 2 — Individual Gene Focus

**Description:** Focusing on individual differentially expressed genes rather than gene programs. Individual genes are often confounded by noise, batch effects, and indirect regulation.

**Regev's diagnosis:** "Her emphasis is on the idea that uncovering how genes are organized into modular programs will reveal more about cellular pathology than focusing on individual genes, and make it possible for researchers to measure less and predict more."

**The trap:** Differential expression analysis produces long lists of genes that are hard to interpret and rarely translate directly to drug targets. Individual genes are not the right unit of analysis for complex biology.

**Correction:** Use matrix factorization methods (NMF, topic modeling) to identify gene programs. Programs are more interpretable, more robust, and more translatable than individual genes.

---

## Anti-Pattern 3 — Isolated Atlases

**Description:** Building single-tissue or single-disease atlases without coordinating with other labs to ensure compatibility. Isolated atlases produce "very nice glimmers of light — a thing here, a thing there" that cannot be connected.

**Regev's diagnosis:** "She realized that if the aim was comprehensive knowledge, the approach needed to be coordinated. If each lab were to rely on its own techniques, it would be hard to standardize the computational tools and the resulting data."

**The trap:** Each lab optimizes its own protocols and computational pipelines, producing data that cannot be compared or integrated across labs.

**Correction:** Invest in coordination infrastructure before scaling. Standardize protocols, data formats, and computational pipelines. Build open-source platforms that allow any researcher to access and analyze the data.

---

## Anti-Pattern 4 — Premature Translation

**Description:** Trying to translate single-cell insights into drug targets before the reference maps are built. Without a healthy reference, it is impossible to identify what is specific to disease.

**Regev's diagnosis:** "Single cell genomics is at a similar place to where human genetics was ten years ago." The field needs to build the reference infrastructure before it can reliably translate insights into medicines.

**The trap:** The pressure to show translational relevance leads labs to jump from single-cell observations to drug targets without the intermediate step of building comprehensive references.

**Correction:** Build the reference first. Identify disease-specific cell states by comparison to the healthy reference. Then find the gene programs that define those states. Then identify drug targets.

---

## Anti-Pattern 5 — Ignoring Rare Cell Types

**Description:** Designing experiments with too few cells to detect rare populations. Some of the most biologically important cells are the rarest.

**Regev's diagnosis:** The ionocyte — a rare cell type that primarily expresses CFTR, the gene linked to cystic fibrosis — was only discoverable because Regev's lab was profiling enough cells to find it.

**The trap:** Experiments designed to characterize the most abundant cell types will miss the rare cell types that may be most important for disease.

**Correction:** Design experiments with enough cells to detect populations that represent <1% of the tissue. Use statistical power calculations to determine the minimum cell number needed to detect rare populations.

---

## Anti-Pattern 6 — Ignoring Spatial Context

**Description:** Analyzing single-cell data without considering where cells are located in the tissue. Cell identity and function are shaped by spatial context — neighboring cells, tissue architecture, gradients.

**Regev's diagnosis:** The Human Cell Atlas will reveal "where the cells are located in the body, how many there are, what forms they can take, even the developmental history of different cell types."

**The trap:** Single-cell RNA-seq dissociates cells from their spatial context. Without spatial information, it is impossible to understand how cell states relate to tissue architecture.

**Correction:** Combine single-cell RNA-seq with spatial transcriptomics. Use the single-cell data to define cell types; use the spatial data to understand their organization.

---

## Anti-Pattern 7 — Competitive Rather Than Collaborative Science

**Description:** Racing against other labs to publish single-cell atlases rather than coordinating to build comprehensive references.

**Regev's diagnosis:** Regev is known for building communities of "fellow travellers" who are collaborative rather than competitive. The Human Cell Atlas succeeded because hundreds of labs worked together.

**The trap:** The incentive structure of academic science rewards individual labs for publishing first, not for building shared resources. This leads to fragmented, incompatible atlases.

**Correction:** Build collaborative communities. Share data before publication. Coordinate protocols and computational pipelines. The value of a reference is proportional to its comprehensiveness — and comprehensiveness requires collaboration.
