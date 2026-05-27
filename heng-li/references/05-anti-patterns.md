# Heng Li — Anti-Patterns

## Anti-Pattern 1 — Using BWA for long reads
BWA is designed for short reads (< 200 bp). For long reads (PacBio, Nanopore), use minimap2. Using BWA for long reads produces incorrect alignments.

## Anti-Pattern 2 — Not sorting and indexing BAM files
Many downstream tools require sorted, indexed BAM files. Always sort with `samtools sort` and index with `samtools index` before downstream analysis.

## Anti-Pattern 3 — Ignoring alignment quality scores
Alignment quality scores (MAPQ) indicate the confidence of each alignment. Low MAPQ reads should be filtered before variant calling. Always filter by MAPQ.

## Anti-Pattern 4 — Using Python for performance-critical code
Python is too slow for genomics-scale data. Use C, C++, or Rust for performance-critical code.

## Anti-Pattern 5 — Not using the right preset for minimap2
minimap2 has presets for different data types (-x sr, -x map-pb, -x map-ont). Using the wrong preset produces suboptimal alignments.

## Anti-Pattern 6 — Releasing software without documentation
A tool without documentation is not a contribution. Always write a README, a man page, and usage examples.

## Anti-Pattern 7 — Not maintaining software
Software that is not maintained becomes obsolete and unreliable. Active maintenance is as important as initial release.
