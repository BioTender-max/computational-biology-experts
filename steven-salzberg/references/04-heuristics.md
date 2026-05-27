# Steven Salzberg — Heuristics

1. Use HISAT2 for RNA-seq alignment — it handles splicing correctly and is fast.
2. Use StringTie for transcript assembly — it produces accurate transcript models.
3. Use Kraken2 for metagenomic classification — it's fast and accurate.
4. Use QUAST for assembly assessment — it provides comprehensive quality metrics.
5. Use BUSCO for gene completeness — it checks whether expected genes are present.
6. Validate tools on real data — don't rely solely on benchmarks.
7. Check for contamination in metagenomic samples — always include human DNA in the database.
8. Use a comprehensive reference database for Kraken — include all relevant organisms.
9. Use the HISAT2-StringTie-Ballgown pipeline — it's the standard for RNA-seq analysis.
10. Assess alignment rate — low alignment rate indicates a problem with the data or the reference.
11. Use multiple quality metrics — don't rely on a single metric.
12. Be skeptical of surprising results — check for technical artifacts before interpreting.
13. Use a reference annotation for StringTie — it improves transcript assembly accuracy.
14. Use the --merge option in StringTie — it produces a consistent annotation across samples.
15. Use Bracken for abundance estimation — it corrects for k-mer length bias in Kraken.
16. Validate key findings with independent methods — don't rely on a single tool.
17. Check for batch effects — they can confound RNA-seq analysis.
18. Use appropriate normalization — RPKM, FPKM, and TPM have different properties.
19. Be critical of inflated claims — many bioinformatics tools are oversold.
20. Publish negative results — they are as important as positive results.
