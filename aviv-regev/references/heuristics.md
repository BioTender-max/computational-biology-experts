# Aviv Regev — Heuristics

20 actionable heuristics across 5 categories, distilled from MIT Technology Review, EMBO, AACR 2024, Broad Institute talks, BioCentury interview, and GV podcast.

---

## Category A — Experimental Design

**H1. Maximize Cell Number Before Depth**
For most single-cell questions, profiling more cells at lower depth yields more information than profiling fewer cells at higher depth. The Miro principle: structure is recognizable from a sample.

**H2. Profile Rare Cell Types Explicitly**
Rare cell types are only discoverable with large sample sizes. Design experiments with enough cells to detect populations that represent <1% of the tissue. The most biologically important cells are often the rarest.

**H3. Use CRISPR for Perturbation Validation**
Computational models of gene networks must be validated by perturbation experiments. CRISPR screens are the gold standard for testing whether a gene is essential for a cellular state or response.

**H4. Combine Single-Cell with Spatial**
Single-cell RNA-seq tells you what cells are doing; spatial transcriptomics tells you where they are. Combine both to understand how cell states relate to tissue architecture.

**H5. Sample Across Patients, Not Just Cells**
Biological heterogeneity across patients is as important as heterogeneity across cells. Design studies with enough patient diversity to capture the range of disease states.

---

## Category B — Computational Analysis

**H6. Find Gene Programs, Not Just DEGs**
Differentially expressed genes are a starting point, not an answer. Use NMF, topic modeling, or other matrix factorization methods to identify co-expression modules that represent gene programs.

**H7. Build the Healthy Reference First**
Before analyzing disease, build a reference of healthy cell states. Disease is deviation from the reference — you can't identify deviation without a baseline.

**H8. Use Trajectory Analysis for Developmental Questions**
Cell differentiation is a continuous process, not a discrete set of states. Use trajectory analysis (Palantir, Monocle, etc.) to understand how cells transition between states.

**H9. Integrate Across Datasets**
Single-cell datasets from different labs, technologies, and conditions can be integrated to build more comprehensive references. Use batch correction and integration methods to combine datasets.

**H10. Validate Computationally Predicted Cell Types Experimentally**
Computational cell type assignments must be validated by orthogonal methods (immunofluorescence, flow cytometry, functional assays). A cell type that exists only in the data is not a cell type.

---

## Category C — Consortium Building

**H11. Standardize Protocols Before Scaling**
Before recruiting hundreds of labs to a consortium, standardize the experimental protocols and computational pipelines. Inconsistent methods produce incomparable data.

**H12. Build Open-Source Platforms**
The value of a reference is proportional to its accessibility. Build open-source computational platforms that allow any researcher to access and analyze the data.

**H13. Recruit Tissue Experts**
No single lab can profile every tissue. Recruit experts in each tissue type to lead the profiling of their tissue. The Human Cell Atlas succeeded by distributing expertise.

**H14. Define Cell Types Conceptually Before Measuring**
Before profiling a tissue, work with domain experts to define what cell types are expected. This guides the experimental design and the computational analysis.

**H15. Publish Data Before Papers**
Make data available to the community before the analysis papers are published. The value of a reference is in its use, not in the publication.

---

## Category D — Translation to Medicine

**H16. Map Disease States, Not Just Disease Genes**
Drug targets are not genes — they are cellular states. Map the cell states that are specific to disease, then find the genes that are essential for those states.

**H17. Use Single-Cell to Stratify Patients**
Different patients have different cellular compositions of their tumors or diseased tissues. Use single-cell data to stratify patients by cellular composition, not just by mutation profile.

**H18. Look for Pre-Existing Resistance**
Regev's melanoma work showed that some cells are resistant to therapy from the start. Before designing a treatment, ask: are there pre-existing resistant cell states? If so, the treatment must address them.

---

## Category E — Career and Leadership

**H19. Create a Vector Field, Not a Directive**
When leading a large team, define the shared vision and standards. Then trust team members to make autonomous decisions within that framework. A vector field is more scalable than individual direction.

**H20. Build Collaborative, Not Competitive, Communities**
Regev is known for building communities of "fellow travellers" who are collaborative rather than competitive. The Human Cell Atlas succeeded because hundreds of labs worked together rather than racing against each other.
