# Aviv Regev — Core Principles

Frequency-ranked from MIT Technology Review profile, EMBO profile, AACR 2024 lecture, Broad Institute talks, Nautilus essay, BioCentury interview, and GV podcast.

---

## Principle 1 — The Cell Is the Unit of Life (★★★★★)

**Frequency:** Every major interview, lecture, and profile.

Regev's foundational belief: the cell is the fundamental unit of biology. Everything we want to understand about health and disease — gene expression, signaling, development, cancer — must ultimately be understood at the level of individual cells. Bulk measurements that average across millions of cells obscure the heterogeneity that drives biology.

> "The basic unit of life is the cell: each of us is made up of around 37 trillion of them and they come in many different types and subtypes like neurons, immune cells, muscle cells, and fat cells."

> "Every cell is an experiment now."

**Implication:** Before designing any genomics experiment, ask: do I need single-cell resolution? In most cases involving complex tissues, the answer is yes.

---

## Principle 2 — Quantity Enables Quality (★★★★★)

**Frequency:** EMBO profile, MIT Tech Review, multiple talks.

Regev's counterintuitive insight: profiling more cells at lower depth often yields more information than profiling fewer cells at higher depth. The Miro painting analogy: you can recognize the painting long before every pixel is filled. Breadth of sampling reveals structure that depth of measurement cannot.

> "Single-cell biology can be most informative if a larger number of cells are profiled at lesser depth, rather than a smaller number at greater depth."

**Implication:** When designing single-cell experiments, optimize for the number of cells profiled, not just the depth of sequencing per cell. Rare cell types are only discoverable with large sample sizes.

---

## Principle 3 — Build the Reference Map First (★★★★★)

**Frequency:** MIT Tech Review, Nautilus, AACR, Broad Institute talks.

Before studying disease, you need to know what normal looks like. The Human Cell Atlas is the reference map that makes it possible to identify what has gone wrong in disease. Just as the periodic table made it possible to predict undiscovered elements, the Human Cell Atlas will make it possible to predict undiscovered cell types.

> "The final product will amount to nothing less than a 'periodic table of our cells,' a tool that is designed not to answer one specific question but to make countless new discoveries possible."

> "Without an atlas of our cells, we don't really know what we're made of."

**Implication:** Invest in reference resources before asking disease-specific questions. The reference pays dividends across all downstream questions.

---

## Principle 4 — Gene Programs, Not Individual Genes (★★★★★)

**Frequency:** BioCentury interview, AACR 2024, multiple talks.

Individual genes are rarely the right unit of analysis. Genes are organized into modular programs — co-regulated modules that represent cellular states, responses, and identities. Programs are more interpretable, more robust, and more translatable than individual genes.

> "Her emphasis is on the idea that uncovering how genes are organized into modular programs will reveal more about cellular pathology than focusing on individual genes, and make it possible for researchers to measure less and predict more."

**Implication:** When analyzing single-cell data, look for gene programs, not just differentially expressed genes. Programs reveal the underlying biology; individual genes are often confounded by noise.

---

## Principle 5 — Design for Inference (★★★★★)

**Frequency:** "Design for inference and massively parallel single cell -omics" podcast, multiple talks.

Regev's principle of "design for inference" means choosing experimental designs that maximize the information you can extract, not just the data you can generate. The question is not "what can I measure?" but "what can I infer from what I measure?"

> "From single cells to international consortia and from striving despite fear to creating a 'vector field' to inspire teams working in sync."

**Implication:** Before running an experiment, ask: what inference do I want to make? What is the minimum data needed to make that inference? Design the experiment to maximize inferential power, not data volume.

---

## Principle 6 — Perturb to Validate (★★★★☆)

**Frequency:** MIT Tech Review, multiple papers.

Computational models of gene networks are only as good as their predictions. Regev validates her models by perturbation experiments — silencing genes, applying stimuli, and checking whether the model's predictions hold. A model that can't predict perturbation outcomes is not a model of the mechanism.

> "Just as someone might study a computer by cutting out circuits and seeing how that changes the machine's operation, Regev tests her model by seeing if it can predict what will happen when she silences specific genes and then exposes the cells to the same stimulus."

**Implication:** Build perturbation validation into your computational workflow. CRISPR screens, RNAi, and chemical perturbations are not just experimental tools — they are the ground truth for computational models.

---

## Principle 7 — Rare Cells Matter (★★★★☆)

**Frequency:** MIT Tech Review, EMBO, AACR.

Some of the most biologically important cells are the rarest. The ionocyte — a rare cell type that primarily expresses CFTR, the gene linked to cystic fibrosis — was discovered by Regev's lab precisely because they were profiling enough cells to find it. Rare cells are only discoverable with large sample sizes.

> "In mapping cells of the lungs, Regev and Jay Rajagopal's lab at Massachusetts General Hospital found a new, very rare cell type that primarily expresses a gene linked to cystic fibrosis."

**Implication:** Don't assume that the most abundant cell types are the most important. Design experiments with enough cells to detect rare populations. The biology of rare cells is often disproportionately important.

---

## Principle 8 — Coordinate to Connect (★★★★☆)

**Frequency:** MIT Tech Review, Human Cell Atlas white paper.

Individual labs producing "very nice glimmers of light — a thing here, a thing there" cannot build a comprehensive reference. Coordination is required to standardize methods, share data, and connect findings across labs and tissues.

> "She realized that if the aim was comprehensive knowledge, the approach needed to be coordinated. If each lab were to rely on its own techniques, it would be hard to standardize the computational tools and the resulting data."

**Implication:** For large-scale reference projects, invest in coordination infrastructure: shared protocols, data standards, computational platforms. The value of a reference is proportional to its comprehensiveness.

---

## Principle 9 — Single-Cell Genomics Is Where Human Genetics Was 10 Years Ago (★★★★☆)

**Frequency:** GV podcast, BioCentury interview.

Regev's conviction: single-cell genomics is at the same inflection point that human genetics was a decade ago — about to transform drug development. The insights from single-cell biology will reshape how drugs are discovered, developed, and targeted.

> "Single cell genomics is at a similar place to where human genetics was ten years ago, and I can't imagine a better person than Aviv to lead us on this journey."
   — Anthony Philippakis, GV

**Implication:** Invest in single-cell genomics capabilities now, before the field matures. The early movers in human genetics built the infrastructure that enabled the GWAS era; the early movers in single-cell genomics will build the infrastructure for the next era of drug discovery.

---

## Principle 10 — Abstractions and Details Are Both Essential (★★★★☆)

**Frequency:** a16z podcast description, multiple profiles.

Regev's intellectual identity is defined by a rare combination: deep love of mathematical abstraction and obsessive attention to biological detail. She does not choose between theory and experiment — she insists on both.

> "Aviv's love of both abstractions and details led her to biology."
   — a16z podcast description

**Implication:** Don't choose between computational and experimental biology. The most powerful insights come from the interplay between mathematical models and experimental validation. Build teams that span both.
