# Lior Pachter — Conceptual Frameworks

## Framework 1: The Pseudoalignment Paradigm
**Problem**: RNA-seq quantification requires knowing which transcripts each read came from.
**Old approach**: Align reads to genome/transcriptome → count alignments.
**Pachter's insight**: You don't need coordinates — only compatibility. Which transcripts is this read consistent with?
**Key abstraction**: Equivalence classes (sets of transcripts compatible with a read) replace alignment coordinates.
**Result**: 100x speedup, comparable accuracy, runs on a laptop.
**Generalization**: Pseudoalignment applies to metagenomics, long-read sequencing (lr-kallisto), and single-cell RNA-seq.

## Framework 2: Inferential vs. Biological Variance Decomposition
**Problem**: Differential expression methods report false positives because they conflate two sources of variance.
**Inferential variance**: Uncertainty in the quantification itself (due to multi-mapping reads). Estimated by bootstrapping the EM algorithm.
**Biological variance**: True differences between biological replicates. Estimated from replicate samples.
**sleuth's solution**: A linear model that explicitly separates the two, using bootstraps as proxies for technical replicates.
**Key insight**: The standard Poisson assumption for RNA-seq technical variance is empirically false.

## Framework 3: The Lightweight Algorithm Philosophy
**Principle**: Algorithms should make frugal use of data, respect constant factors, and work with small units of data where possible.
**Application**: Replace approximate alignment of reads with exact matching of k-mers (Sailfish) → replace k-mer alignment with compatibility checking (kallisto).
**Generalization**: Ask "what is the minimum information needed?" before designing any algorithm.

## Framework 4: Interactive Analysis as Epistemology
**Old model**: Submit job to cluster → wait days → get result → frozen analysis.
**New model**: Run on laptop in minutes → explore → re-quantify → iterate.
**Implication**: Fast tools change what questions biologists ask. Interactive analysis enables hypothesis generation, not just hypothesis testing.
