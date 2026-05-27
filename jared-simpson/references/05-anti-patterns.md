# Jared Simpson — Anti-Patterns

## Anti-Pattern 1 — Discarding signal-level data after base calling
The raw electrical signal contains more information than the base-called sequence. Don't discard it — store the pod5/fast5 files for future analysis.

## Anti-Pattern 2 — Using bisulfite sequencing when nanopore is available
Bisulfite sequencing is destructive and introduces biases. Nanopore sequencing can detect methylation directly, without chemical treatment.

## Anti-Pattern 3 — Using short-read tools for nanopore data
Short-read tools (BWA, GATK) are not designed for nanopore data. Use minimap2 for alignment and Medaka or Nanopolish for variant calling.

## Anti-Pattern 4 — Not validating on known sequences
Nanopore analysis algorithms should be validated on sequences where the truth is known before applying to unknown samples.

## Anti-Pattern 5 — Ignoring the error profile
Nanopore errors are different from Illumina errors — they are more likely to be insertions and deletions, especially in homopolymer regions. Use tools designed for nanopore error profiles.

## Anti-Pattern 6 — Not using real-time analysis for infectious disease surveillance
Nanopore sequencers produce data in real time. Not using real-time analysis for infectious disease surveillance wastes the key advantage of nanopore sequencing.

## Anti-Pattern 7 — Using outdated base callers
Base calling accuracy has improved dramatically with each generation of Oxford Nanopore's software. Always use the latest base caller (Dorado) for the best accuracy.
