# Bonnie Berger — Conceptual Frameworks

## Framework 1: Compressive Genomics
**Problem**: Genomic databases are growing faster than compute can handle.
**Insight**: Biological sequences are not random — they cluster in dense groups (evolutionary tree is not too bushy). This redundancy can be exploited.
**Method**: Compress data so computation can be performed directly on the compressed representation. Two-stage coarse/fine search: coarse search on representative sequences; fine search only on those within threshold of query.
**Result**: 100x+ speedup on BLAST/BLAT while retaining >99% accuracy. Runtime scales with unique data, not total data.
**Generalization**: Compressive omics — protein databases (CaBLASTP), metagenomics, chemogenomics, NGS read mapping.

## Framework 2: Network Alignment (IsoRank / Mashup)
**Insight**: Two genes are likely homologs if their interaction partners are also homologs (PageRank-like reasoning). Network topology provides orthogonal information to sequence similarity.
**IsoRank**: Aligns protein-protein interaction networks across species. Two regions are a good match if their neighbors are alike, and their neighbors' neighbors, and so on.
**Mashup**: Integrates heterogeneous data sources (transcriptomics, proteomics, pharmacogenomics, experimental data) through a common network lens.
**Application**: Predicting gene function, identifying disease pathways, drug repurposing.

## Framework 3: Genomic Privacy via Multi-Party Computation
**Problem**: Sensitive genomic data cannot be shared across institutions without privacy risk.
**Solution**: Multi-party computation (from cryptography) allows institutions to jointly train models on encrypted data without revealing it to each other.
**Application**: Drug-target interaction prediction across pharmaceutical companies; secure crowdsourcing of genomic data.
**Key insight**: Cryptographic techniques developed for financial privacy are directly applicable to biological data privacy.

## Framework 4: "Mad Libs for Viruses" — Language Models for Viral Escape
**Insight**: Protein sequences have syntax (structural viability) and semantics (immune recognition). Language models trained on protein sequences can predict whether a new variant will escape immune recognition.
**Method**: Swap subsets of amino acids; grammatically incorrect variants are structurally non-viable; semantically distant but grammatically correct variants are dangerous.
**Application**: Predicting immune escape for influenza, HIV, SARS-CoV-2.
**Key quote**: "To have a really funny Mad Lib, you need enough change in meaning."

## Framework 5: Compressed Sensing for Transcriptomics
**Insight**: Gene expression data has sparse, modular structure. This means it can be recovered from far fewer measurements than the number of genes.
**Method**: Composite measurements — linear combinations of gene expression levels — can capture the same information as full transcriptome profiling in ~100 dimensions instead of 20,000.
**Application**: Efficient experimental design for transcriptomics; dimensionality reduction that preserves biological signal.
