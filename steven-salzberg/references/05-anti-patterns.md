# Steven Salzberg — Anti-Patterns

## Anti-Pattern 1 — Using TopHat for RNA-seq alignment
TopHat is outdated — use HISAT2 instead. HISAT2 is faster, more accurate, and uses less memory.

## Anti-Pattern 2 — Ignoring splicing in RNA-seq analysis
RNA-seq reads span exon-exon junctions. Tools that don't handle splicing correctly will misalign reads and produce incorrect expression estimates.

## Anti-Pattern 3 — Using a small database for Kraken
Kraken's accuracy depends on the completeness of the database. Using a small database will miss many organisms and produce incorrect classifications.

## Anti-Pattern 4 — Ignoring contamination in metagenomic samples
Metagenomic samples are contaminated with human DNA, reagent DNA, and environmental DNA. Always check for contamination before interpreting results.

## Anti-Pattern 5 — Treating genome annotations as definitive
Genome annotations are continuously updated. Don't treat any annotation as definitive — check the version and date of the annotation you are using.

## Anti-Pattern 6 — Relying solely on benchmarks
Benchmarks are useful but limited. Always validate tools on real data from the organism of interest.

## Anti-Pattern 7 — Ignoring methodological flaws in widely-used tools
Many widely-used bioinformatics tools have methodological flaws. Don't assume that a tool is correct just because it is widely used.
