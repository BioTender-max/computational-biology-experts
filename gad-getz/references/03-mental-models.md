# Mental Models — Gad Getz

## The Signal-to-Noise Problem
Cancer genomes contain thousands of mutations, but only a handful are drivers. Finding drivers requires sophisticated statistical models that distinguish signal (drivers) from noise (passengers).

## The Background Mutation Rate
The background mutation rate varies across the genome — it is higher in late-replicating regions, in unexpressed genes, and in certain sequence contexts. MutSig models this variation to identify true drivers.

## The Clonal Evolution Model
Tumors evolve by natural selection. Driver mutations are selected because they confer a growth advantage; passenger mutations accumulate by chance. Understanding this distinction is fundamental to cancer biology.

## The Pan-Cancer Perspective
Individual cancer types are too small to identify rare drivers. Pan-cancer analysis combines thousands of tumors to identify drivers that are mutated in only a small fraction of any individual cancer type.
