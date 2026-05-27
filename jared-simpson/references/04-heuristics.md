# Jared Simpson — Heuristics

1. Work at the signal level when possible — base calling discards information.
2. Use Nanopolish for consensus calling — it's more accurate than base-level methods.
3. Use Nanopolish for methylation detection — it doesn't require bisulfite conversion.
4. Use the ARTIC protocols for viral genome sequencing — they are optimized for nanopore.
5. Use real-time analysis for infectious disease surveillance — it enables faster decisions.
6. Validate on known sequences — test the algorithm before applying to unknown samples.
7. Use HMMs for signal interpretation — they are the right framework for noisy data.
8. Use miniasm for rapid long-read assembly — it's fast and doesn't require error correction.
9. Use Medaka or Nanopolish for polishing — they improve assembly accuracy.
10. Use direct RNA sequencing for modification detection — it doesn't require chemical treatment.
11. Use Nextclade for variant classification — it's fast and accurate for viral variants.
12. Use the latest base caller — Dorado (Oxford Nanopore) is the current best.
13. Use the appropriate pore chemistry — R10.4.1 provides the best accuracy.
14. Use ultra-long reads for complex regions — they can span centromeres and other difficult regions.
15. Use adaptive sampling for targeted sequencing — it enriches for regions of interest.
16. Validate methylation calls with bisulfite sequencing — for critical applications.
17. Use the signal-level data (pod5/fast5) — don't discard it after base calling.
18. Use Snakemake or Nextflow for pipeline management — they enable reproducible workflows.
19. Share protocols and tools openly — the nanopore community benefits from open science.
20. Consider the error profile — nanopore errors are different from Illumina errors.
