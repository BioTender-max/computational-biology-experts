# Heng Li — Conceptual Frameworks

## Framework 1 — BWT/FM-index for Short-Read Alignment
The Burrows-Wheeler Transform enables O(n) alignment of short reads. BWA uses the FM-index (compressed BWT) to align billions of reads per day. BWA-MEM extends this to longer reads using seed-and-extend.
**Tools**: BWA, BWA-MEM, BWA-MEM2

## Framework 2 — Minimizer-Based Seeding for Long-Read Alignment
Long reads are too long for BWT-based alignment. minimap2 uses minimizers — the lexicographically smallest k-mer in a window — to seed alignments. Sparse but representative.
**Tools**: minimap2 (use -x preset for data type)

## Framework 3 — Phased Assembly Graphs for HiFi Assembly
HiFi reads are long (10–25 kb) and accurate (>99.9%). hifiasm uses phased assembly graphs to produce haplotype-resolved assemblies, maintaining both haplotypes as separate paths.
**Tools**: hifiasm (--h1/--h2 for trio binning, Hi-C for phasing)

## Framework 4 — The SAM/BAM Format
Universal format for storing sequence alignments. BAM is the binary, compressed version. SAMtools provides a comprehensive toolkit for manipulation.
**Tools**: SAMtools, BCFtools, htslib

## Framework 5 — The GFA Format for Assembly Graphs
Graphical Fragment Assembly format represents assembly graphs, enabling interoperability between assemblers and downstream tools.
**Tools**: Bandage (visualization), vg (graph alignment), Minigraph-Cactus
