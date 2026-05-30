# Heuristics — Núria López-Bigas

1. **Always model the background before calling drivers** — a gene with many mutations in a high-mutation-rate region is not necessarily a driver; compare to the expected rate given chromatin context and trinucleotide composition.

2. **Combine orthogonal signals** — if two independent methods (e.g., clustering + functional impact bias) both flag a gene, confidence is multiplicatively higher than either alone. Genes flagged by only one method require additional validation.

3. **Use cohort size as a quality filter** — driver detection is unreliable in cohorts smaller than ~100 tumors; below this threshold, false discovery rates are unacceptably high. Report confidence intervals on driver lists.

4. **Distinguish gene-level from mutation-level drivers** — knowing that TP53 is a driver gene does not tell you which specific TP53 mutations are drivers; BoostDM addresses the second question, which is what matters clinically.

5. **Annotate by tissue type** — a mutation that drives lung cancer may be a passenger in colon cancer; driver status is gene × tissue specific, not universal. Always specify the cancer type when reporting driver status.

6. **Treat the non-coding genome as a frontier, not a wasteland** — apply the same positive selection logic to promoters, UTRs, and lncRNAs; the methods work, the data is just harder to interpret due to limited functional annotation.

7. **Validate computationally predicted drivers with orthogonal evidence** — functional experiments, structural data, and clinical outcomes all provide independent validation of computational predictions. Computational prediction is hypothesis generation, not proof.

8. **Build tools that clinicians can use** — a driver prediction that requires a bioinformatician to interpret is not yet a clinical tool; the interface and output format matter as much as the algorithm.

9. **Make data and tools open** — the compendium of cancer drivers is a community resource; restricting access slows the entire field. Publish tools, databases, and pipelines alongside papers.

10. **Track mutational footprints of treatments** — chemotherapy leaves a mutational signature in tumor genomes; quantifying this signature enables assessment of treatment-induced mutation burden and secondary cancer risk.

11. **Sequence matched normal tissue** — comparing tumor to matched normal tissue from the same patient is essential for accurate somatic mutation calling; germline variants must be subtracted.

12. **Apply cancer genomics methods to pre-malignant conditions** — the same positive selection logic that identifies cancer drivers applies to clonal hematopoiesis and other pre-malignant clonal expansions; repurpose existing methods rather than building from scratch.
