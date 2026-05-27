# Jared Simpson — Conceptual Frameworks

## Framework 1 — Signal-Level Analysis with Hidden Markov Models
Nanopore sequencers measure electrical current as DNA passes through a nanopore. The current depends on the k-mer in the pore. Nanopolish uses an HMM to model the relationship between DNA sequence and electrical signal.
**Tools**: Nanopolish (consensus calling, methylation detection, SNP calling)

## Framework 2 — String Graph Assembly
The string graph represents overlap relationships between reads as a graph. Assembly = finding a path through this graph representing the genome.
**Tools**: SGA (short reads), miniasm (long reads)

## Framework 3 — Direct RNA Sequencing
Nanopore sequencers can sequence RNA directly — without reverse transcription or amplification. Enables detection of RNA modifications, full-length transcript sequencing, and direct measurement of RNA abundance.
**Tools**: Nanopolish (RNA-specific models), Dorado (base calling)

## Framework 4 — Real-Time Genomic Surveillance
Nanopore sequencers produce data in real time. Real-time analysis algorithms can identify pathogens, track mutations, and alert public health officials before the sequencing run is complete.
**Tools**: ARTIC protocols, Nanopolish, Nextclade

## Framework 5 — Methylation Detection without Bisulfite Conversion
Nanopore sequencing can detect DNA methylation directly — the electrical signal is different for methylated and unmethylated bases. Nanopolish uses a trained HMM to distinguish methylated from unmethylated bases.
**Tools**: Nanopolish call-methylation; Dorado (with modification models)
