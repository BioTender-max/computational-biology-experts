# Computational Biology Experts — Skill Library

A curated library of expert reasoning frameworks for 13 landmark computational biologists. Each package is distilled from primary sources: interviews, lectures, landmark papers, blog posts, and award speeches.

## Scientists

| Scientist | Domain | Key Contributions |
|-----------|--------|-------------------|
| [David Baker](./david-baker/) | Protein Design | Rosetta, RFDiffusion, de novo protein design |
| [Demis Hassabis](./demis-hassabis/) | AI for Biology | AlphaFold, DeepMind, Nobel Prize 2024 |
| [Eugene Myers](./eugene-myers/) | Genome Assembly | BLAST, string graph assembly, whole-genome shotgun |
| [Aviv Regev](./aviv-regev/) | Single-Cell Genomics | scRNA-seq, Human Cell Atlas, Genentech R&D |
| [Lior Pachter](./lior-pachter/) | Computational Genomics | kallisto, sleuth, pseudoalignment |
| [Bonnie Berger](./bonnie-berger/) | Mathematical Biology | Compressive genomics, IsoRank, privacy-preserving genomics |
| [Ewan Birney](./ewan-birney/) | Genome Annotation | Ensembl, ENCODE, GeneWise, EMBL-EBI |
| [Søren Brunak](./soren-brunak/) | Disease Systems Biology | SignalP, disease trajectories, EHR analysis |
| [Christina Leslie](./christina-leslie/) | ML for Genomics | String kernels, GraphReg, regulatory genomics |
| [Bernhard Schölkopf](./bernhard-scholkopf/) | ML / Causal Inference | SVMs, kernel methods, causal representation learning |
| [Dana Pe'er](./dana-peer/) | Single-Cell / Cancer | Wanderlust, Palantir, MAGIC, cellular plasticity |
| [Manolis Kellis](./manolis-kellis/) | Comparative Genomics | ChromHMM, ENCODE, Alzheimer's immune basis, FTO locus |
| [Eran Segal](./eran-segal/) | Personalized Medicine | Personalized nutrition, microbiome, nucleosome positioning |

## Package Structure

Each scientist's folder contains:

```
<scientist-name>/
├── SKILL.md              # Main skill file: identity, 6-step protocol, principles, frameworks, heuristics, anti-patterns, quotes
├── avatar.png            # AI-generated portrait
└── references/
    ├── principles.md     # Core principles ranked by frequency
    ├── frameworks.md     # Conceptual frameworks with methods
    ├── mental-models.md  # Key mental models and metaphors
    ├── heuristics.md     # Practical rules (20 per scientist)
    ├── anti-patterns.md  # Failure modes to avoid
    ├── quotes.md         # Verified quotes with sources
    └── sources.md        # Primary sources used
```

## Methodology

Each skill package was distilled using the following pipeline:
1. **Source discovery**: WebSearch across 8 intent buckets (essays, talks, interviews, frameworks, papers, lab philosophy, books, award lectures)
2. **Fetch & extract**: Full text from top ~15 sources per scientist
3. **Literature search**: Landmark papers via PubMed/Consensus
4. **Distillation**: Structured extraction of principles, frameworks, mental models, heuristics, anti-patterns, and quotes
5. **Clustering & ranking**: Merge duplicates, rank by cross-source frequency
6. **Authoring**: SKILL.md + 7 reference files per scientist
7. **Avatar generation**: AI-generated painterly portrait

## Usage

These skill packages are designed to be loaded as expert reasoning frameworks. When working on a computational biology problem, load the relevant scientist's skill to reason in their mode:

- **Trajectory analysis / single-cell**: Dana Pe'er, Aviv Regev
- **Genome assembly / algorithms**: Eugene Myers
- **RNA-seq / statistical genomics**: Lior Pachter
- **Epigenomics / disease mechanisms**: Manolis Kellis, Ewan Birney
- **Personalized medicine / microbiome**: Eran Segal
- **Machine learning for biology**: Christina Leslie, Bernhard Schölkopf, Bonnie Berger
- **Protein design / structure**: David Baker, Demis Hassabis
- **Disease systems biology**: Søren Brunak
