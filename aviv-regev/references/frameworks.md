# Aviv Regev — Frameworks

Five structured frameworks extracted from MIT Technology Review, EMBO, AACR 2024, Broad Institute talks, and BioCentury interview.

---

## Framework 1 — Cell as Computer

**Source:** MIT Technology Review profile, Broad Institute talks

Regev's foundational metaphor for understanding cellular biology: a cell is a complex computer made of millions of interacting molecules. Proteins on the cell surface receive molecular messages; these are relayed to proteins in the nucleus; the nucleus responds by transcribing DNA; new proteins are produced; new signals are sent.

**The architecture:**
- **Input layer:** Surface receptors receiving molecular signals (glucose, pathogens, hormones)
- **Processing layer:** Signaling networks relaying and transforming signals
- **Memory layer:** Chromatin state encoding cellular history
- **Output layer:** Gene expression programs producing proteins and behaviors

**The circuit analogy:**
- Protein signaling networks are "circuits"
- The cell can be thought of "almost like a wiring diagram"
- Understanding the cell requires understanding the circuit topology

**Why this matters:**
- It makes the cell tractable for computational analysis
- It suggests that perturbation experiments (cutting circuits) are the right way to validate models
- It implies that disease is a circuit malfunction — and that drugs are circuit interventions

**Key quote:** "It's like a complex computer that is made of these many, many different parts that are interacting with each other and telling each other what to do."

---

## Framework 2 — The Periodic Table of Cells

**Source:** MIT Technology Review, Nautilus essay, Human Cell Atlas white paper

Regev's vision for the Human Cell Atlas: a reference map of all human cells that is to biology what the periodic table is to chemistry — not an answer to a specific question, but a framework that makes countless new discoveries possible.

**The analogy:**
- Periodic table: organized elements by properties → predicted undiscovered elements
- Human Cell Atlas: organized cells by molecular identity → will predict undiscovered cell types

**What the atlas provides:**
1. **Cell type catalog:** All ~37 trillion cells organized by molecular identity
2. **Spatial map:** Where each cell type is located in the body
3. **Developmental history:** How each cell type differentiated from stem cells
4. **Disease deviation:** How cell states change in disease

**The Google Maps interface:**
- Zoom in to molecular level (gene expression in individual cells)
- Zoom out to tissue and organ level
- Navigate between healthy and disease states

**The sampling insight:**
You don't need to sequence all 37 trillion cells. Like Van Gogh's Starry Night becoming recognizable long before every pixel is filled, the atlas can give a complete picture from a representative sample.

**Key quote:** "The final product will amount to nothing less than a 'periodic table of our cells,' a tool that is designed not to answer one specific question but to make countless new discoveries possible."

---

## Framework 3 — Gene Programs

**Source:** BioCentury interview, AACR 2024, multiple papers

Regev's framework for analyzing single-cell data: instead of focusing on individual differentially expressed genes, identify the modular gene programs that represent cellular states, responses, and identities.

**What is a gene program?**
- A co-regulated module of genes that are expressed together
- Represents a cellular function, state, or response
- More interpretable than individual genes
- More robust to noise
- More translatable to drug targets

**Why programs beat individual genes:**
- Individual genes are often confounded by noise, batch effects, and indirect regulation
- Programs represent the underlying biology, not just the measurement
- Programs can be compared across cell types, tissues, and species
- Programs reveal the modular architecture of cellular function

**The translational implication:**
"Uncovering how genes are organized into modular programs will reveal more about cellular pathology than focusing on individual genes, and make it possible for researchers to measure less and predict more."

**Application:**
1. Run single-cell RNA-seq on cells of interest
2. Identify co-expression modules (NMF, topic modeling, etc.)
3. Characterize each module by its biological function
4. Compare modules across conditions, cell types, and diseases
5. Identify modules that are dysregulated in disease
6. Target the dysregulated module, not individual genes

---

## Framework 4 — Design for Inference

**Source:** "Design for inference and massively parallel single cell -omics" podcast, multiple talks

Regev's experimental design philosophy: choose designs that maximize the information you can extract, not just the data you can generate.

**The key questions:**
1. What inference do I want to make?
2. What is the minimum data needed to make that inference?
3. What experimental design maximizes inferential power?

**The depth vs. breadth tradeoff:**
- More cells at lower depth → better for discovering rare cell types, understanding population structure
- Fewer cells at higher depth → better for understanding individual cell biology in detail
- Regev's insight: for most questions, breadth beats depth

**The Miro painting principle:**
A blank slide fills pixel by pixel with dashes of yellow and red. Long before the picture is complete, viewers can make out Joan Miro's "Painting, March 13, 1933." The structure is recognizable from a sample — you don't need every pixel.

**Application:**
- For cell type discovery: maximize cell number, minimize depth
- For gene regulatory network inference: maximize perturbation diversity
- For disease comparison: maximize patient diversity, not just cell number

---

## Framework 5 — Atlas to Medicine

**Source:** AACR 2024, BioCentury interview, GV podcast

Regev's framework for translating single-cell insights into medicines at Genentech.

**The pipeline:**
1. **Build the atlas** — Map cell types and states in healthy and diseased tissue
2. **Identify disease-specific states** — Find cell states that are present in disease but not in health
3. **Find the gene programs** — Identify the modular programs that define disease states
4. **Validate with perturbations** — CRISPR screens, chemical perturbations
5. **Identify drug targets** — Genes or pathways that are essential for disease states
6. **Design the drug** — Target the disease state without affecting healthy states

**The cancer complexity problem:**
"There are more than 100 cancer cell types, maybe a couple of million cancer patients each year, 10,000 driver mutations, and maybe 10^20 different ways variants can combine. That enormous complexity makes our shared vision of understanding cancer difficult."

**The single-cell solution:**
Single-cell genomics can decompose this complexity by identifying the cell states that matter, the programs that drive them, and the targets that are specific to disease states.

**Key quote:** "Single cell genomics is at a similar place to where human genetics was ten years ago."
