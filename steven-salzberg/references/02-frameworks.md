# Steven Salzberg — Conceptual Frameworks

## Framework 1 — Spliced Alignment for RNA-seq
RNA-seq reads come from spliced mRNA. Aligning them to a genome requires handling exon-exon junctions. HISAT2 uses a graph-based approach to handle splicing efficiently.
**Tools**: HISAT2 (alignment), StringTie (transcript assembly), Ballgown (differential expression)

## Framework 2 — Transcript Assembly and Quantification
StringTie assembles transcripts from RNA-seq alignments using a network flow algorithm to find the minimum number of transcripts explaining observed read coverage.
**Tools**: StringTie (--merge for cross-sample, -e for expression estimation)

## Framework 3 — Exact k-mer Matching for Metagenomics
Kraken classifies metagenomic reads by finding the lowest common ancestor (LCA) of all database sequences sharing a k-mer with the read. Much faster than alignment-based methods.
**Tools**: Kraken2 (classification), Bracken (abundance estimation)

## Framework 4 — Gene Finding with GLIMMER
GLIMMER uses interpolated Markov models to find protein-coding genes in microbial genomes. Trained on known genes, then applied to find new genes.
**Tools**: GLIMMER (microbial), AUGUSTUS (eukaryotic), MAKER (pipeline)

## Framework 5 — Genome Assembly Assessment with QUAST
QUAST assesses assembly quality by comparing to a reference genome or computing reference-free statistics: N50, L50, misassemblies, etc.
**Tools**: QUAST, BUSCO, Merqury
