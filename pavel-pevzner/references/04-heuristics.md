# Pavel Pevzner — Heuristics

1. Formulate the problem mathematically before writing code — the right formulation often reveals the correct algorithm.
2. Use de Bruijn graphs for short-read assembly — they are the correct mathematical framework.
3. Use repeat graphs for long-read assembly — they handle the error profile of long reads.
4. Choose k-mer size carefully — too small = too many false overlaps; too large = miss true overlaps.
5. Error-correct reads before assembly — errors create spurious branches in the de Bruijn graph.
6. Use paired-end reads for repeat resolution — they provide long-range information.
7. Assess assembly quality with QUAST — it provides comprehensive assembly statistics.
8. Use BUSCO to assess gene completeness — it checks whether expected genes are present.
9. Benchmark against existing assemblers — don't claim improvement without comparison.
10. Publish the software — an algorithm without software is not a contribution.
11. Use long reads for complex genomes — short reads cannot resolve long repeats.
12. Consider the ploidy — diploid and polyploid genomes require special handling.
13. Use Hi-C for scaffolding — it provides chromosome-scale information.
14. Validate with optical mapping — it provides independent confirmation of large-scale structure.
15. Think about the repeat structure — understanding the repeat landscape is essential for assembly.
16. Use graph visualization tools — Bandage helps understand assembly graphs.
17. Don't over-polish — excessive polishing can introduce errors.
18. Use multiple assemblers and compare — different assemblers have different strengths.
19. Consider the sequencing technology — the optimal assembler depends on the technology.
20. Teach the algorithms, not just the tools — understanding algorithms enables better use of tools.
