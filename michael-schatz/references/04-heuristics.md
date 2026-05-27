# Michael Schatz — Heuristics

1. Use long reads for structural variant detection — short reads miss most SVs.
2. Use NGMLR for long-read alignment — it's optimized for SV detection.
3. Use Sniffles for SV calling — it's the most accurate tool for long-read SVs.
4. Use phased assembly for diploid genomes — it reveals heterozygous variants.
5. Use Hi-C for chromosome-scale scaffolding — it provides long-range information.
6. Use cloud computing for large-scale genomics — it enables analysis at scales impossible on local clusters.
7. Use Nextflow or Snakemake for workflow management — they enable reproducible pipelines.
8. Use BUSCO for assembly quality assessment — it checks whether expected genes are present.
9. Use Merqury for k-mer-based quality assessment — it provides reference-free quality metrics.
10. Consider the ploidy — polyploid genomes require specialized assembly tools.
11. Use Jasmine for population-scale SV comparison — it enables SV genotyping across cohorts.
12. Use Assemblytics for assembly comparison — it identifies differences between assemblies.
13. Use Scalpel for indel detection — it's accurate for small insertions and deletions.
14. Validate SVs with orthogonal methods — long reads, short reads, and optical mapping.
15. Consider the repeat structure — plant genomes are often highly repetitive.
16. Use the latest sequencing technology — HiFi reads provide the best balance of length and accuracy.
17. Share data and tools openly — open science enables the community to build on the work.
18. Benchmark against existing tools — don't claim improvement without comparison.
19. Consider cancer-specific challenges — tumor genomes are highly rearranged and heterogeneous.
20. Invest in education and community building — they are scientific contributions.
