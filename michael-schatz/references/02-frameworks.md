# Michael Schatz — Conceptual Frameworks

## Framework 1 — Long-Read Structural Variant Detection
Structural variants (SVs) are genomic alterations > 50 bp. Short reads cannot span most SVs; long reads can. Sniffles detects SVs from long-read alignments by identifying reads that span SV breakpoints.
**Tools**: NGMLR (alignment), Sniffles (SV calling), Jasmine (population-scale SV comparison)

## Framework 2 — Phased Diploid Assembly
Phased assembly produces separate assemblies for each haplotype, revealing heterozygous variants. Requires long reads and phasing information (Hi-C or trio data).
**Tools**: hifiasm, FALCON-Unzip, Assemblytics (comparison)

## Framework 3 — Cloud Computing for Genomics
Cloud computing enables genomics analysis at scales impossible on local clusters. Modern cloud genomics uses Kubernetes, Nextflow, and Snakemake.
**Tools**: AWS, Google Cloud, Azure; Nextflow, Snakemake; Terra, DNAnexus

## Framework 4 — Plant Genome Assembly
Plant genomes are often large (1–20 Gb), polyploid, and repeat-rich. Assembly requires long reads, Hi-C scaffolding, and specialized tools for polyploid genomes.
**Tools**: hifiasm, Verkko; Hi-C scaffolding; BUSCO, Merqury

## Framework 5 — Cancer Structural Variant Analysis
Cancer genomes contain thousands of structural variants that drive tumor evolution. Long-read sequencing reveals complex rearrangements that short reads miss.
**Tools**: NGMLR + Sniffles (SV detection), GECCO (non-coding SV analysis), Scalpel (indel detection)
