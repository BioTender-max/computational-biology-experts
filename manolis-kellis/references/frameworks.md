# Manolis Kellis — Conceptual Frameworks

## Framework 1: Comparative Genomics for Functional Element Discovery
**Insight**: Evolution is the most powerful filter for functional elements.

**Method**:
1. Align multiple closely related species (e.g., 12 Drosophila genomes, 4 yeast species)
2. Identify evolutionary signatures: conservation, constraint, acceleration
3. Use signatures to discover functional elements: protein-coding genes, RNA structures, microRNAs, enhancers, regulatory motifs

**Key insight**: Sequences conserved across species are functional; sequences that diverge are not. This is the most powerful filter available for distinguishing signal from noise.

**Landmark**: Proof of ancient whole-genome duplication in yeast (Nature 2004); discovery of functional elements in 12 Drosophila genomes (Nature 2007).

---

## Framework 2: Chromatin State Annotation (ChromHMM)
**Insight**: Chromatin marks reveal the functional state of genomic regions.

**Method**: ChromHMM — hidden Markov model that learns chromatin states from combinations of histone marks:
1. Input: genome-wide histone modification data (ChIP-seq) across multiple marks
2. Model: multivariate HMM with Gaussian emission distributions
3. Output: 15 chromatin states (promoters, enhancers, transcribed regions, repressed regions, etc.)

**Application**: Systematic annotation of the non-coding genome; linking regulatory elements to target genes; identifying cell-type-specific regulatory activity.

**Scale**: 111 reference human epigenomes (Roadmap Epigenomics); ENCODE.

---

## Framework 3: Disease Mechanism Dissection via Epigenomics + GWAS
**Insight**: GWAS variants point to loci; epigenomics reveals the mechanisms.

**Method**:
1. Map GWAS variants to chromatin states (which cell types? which regulatory elements?)
2. Identify enriched cell types and regulatory elements
3. Link regulatory elements to target genes (eQTLs, Hi-C)
4. Identify pathways and mechanisms

**Alzheimer's**: AD risk variants enriched in microglial enhancers → immune basis, not neuronal.
**Obesity (FTO)**: Strongest obesity variant acts via fat cell energy balance switch → not appetite control.

---

## Framework 4: Single-Cell Disease Dissection
**Insight**: Bulk epigenomics averages across cell types; single-cell methods reveal cell-type-specific mechanisms.

**Cell-Projected Phenotypes (CPP)**:
1. Profile millions of single cells from hundreds of individuals
2. Map donor-level clinical variables onto individual cells
3. Reveal intra-individual heterogeneity in disease manifestation
4. Identify disease subtypes with distinct molecular signatures

**Scale**: 3.4 million cells from ~600 Alzheimer's disease donors; 850,000 nuclei from 92 individuals (epigenomic dissection of AD).
