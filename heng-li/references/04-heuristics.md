# Heng Li — Heuristics

1. Use BWA-MEM2 for short-read alignment — it's the fastest and most accurate.
2. Use minimap2 for long-read alignment — use the -x preset for your data type.
3. Use hifiasm for HiFi genome assembly — it produces the best haplotype-resolved assemblies.
4. Use SAMtools for BAM manipulation — sort, index, filter, and statistics.
5. Use BCFtools for variant calling — it's fast and accurate for SNPs and indels.
6. Design data formats before writing tools — a good format enables interoperability.
7. Write C for performance-critical code — Python is too slow for genomics-scale data.
8. Use SIMD instructions for alignment — they provide 4–8× speedup on modern CPUs.
9. Minimize memory allocation — memory allocation is expensive; reuse buffers.
10. Profile before optimizing — don't optimize code that isn't the bottleneck.
11. Use minimizers for long-read seeding — they are sparse but representative.
12. Use phased assembly graphs for diploid genomes — they preserve haplotype information.
13. Use Hi-C data for phasing — it provides long-range haplotype information.
14. Release software on GitHub — it enables community contributions and issue tracking.
15. Write clear documentation — a tool without documentation is not a contribution.
16. Respond to issues — active maintenance is as important as initial release.
17. Use sensible defaults — most users should not need to change parameters.
18. Benchmark against alternatives — don't claim improvement without comparison.
19. Use the right tool for the right data — BWA for short reads, minimap2 for long reads.
20. Think about the next sequencing technology — the computational problems evolve with the technology.
