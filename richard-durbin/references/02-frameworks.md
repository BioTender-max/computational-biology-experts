# Richard Durbin — Conceptual Frameworks

## Framework 1 — The HMM Paradigm for Sequence Analysis
Profile HMMs model protein families as probabilistic state machines with match, insert, and delete states. Each position has position-specific emission probabilities capturing evolutionary constraints. Enables gene finding, protein family detection, RNA structure prediction.

**Tools**: HMMER (protein), Infernal (RNA), Pfam (database), Rfam (database)

## Framework 2 — The Coalescent for Population History
The coalescent model describes how lineages merge backward in time. PSMC uses heterozygosity patterns along a single diploid genome to infer effective population size through time. MSMC extends to multiple genomes for population separations.

**Tools**: PSMC, MSMC, MSMC2

## Framework 3 — The Graph Genome for Structural Variation
Linear reference genomes fail to represent structural variation. Graph genomes represent all known variants as paths through a directed acyclic graph, reducing reference bias.

**Tools**: vg toolkit, Minigraph-Cactus

## Framework 4 — The BWT/FM-index for Efficient Alignment
The Burrows-Wheeler Transform enables O(n) alignment of short reads. The positional BWT (PBWT) extends this to haplotype matching across large cohorts.

**Tools**: BWA, BWA-MEM, BWA-MEM2, PBWT

## Framework 5 — The Darwin Tree of Life Framework
Every species has a genome worth sequencing. Telomere-to-telomere assembly using HiFi long reads + Hi-C scaffolding, validated with BUSCO and Merqury.

**Tools**: hifiasm, Verkko, BUSCO, Merqury
