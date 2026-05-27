# John Novembre — Conceptual Frameworks

## Framework 1 — PCA of Genetic Variation
PCA of a genotype matrix (individuals × SNPs) reveals major axes of genetic variation. The "genes mirror geography" result shows that PC1 and PC2 of European genetic variation correspond to the north-south and east-west axes of Europe.

**Key insight**: Geographic structure arises from isolation by distance — nearby populations exchange more migrants than distant ones.
**Tools**: PLINK, EIGENSOFT; plot PC1 vs. PC2 colored by geographic origin

## Framework 2 — EEMS (Effective Migration Surfaces)
Models effective migration rate across a geographic grid using a Voronoi tessellation. Estimates migration rates between adjacent grid cells by fitting a model to observed genetic distances. Low rates = barriers; high rates = corridors.

**Tools**: EEMS software (github.com/dipetkov/eems)

## Framework 3 — Isolation by Distance
Under isolation by distance, genetic distance increases with geographic distance. Deviations indicate barriers, corridors, or historical events.

**Test**: Mantel test; plot FST/(1-FST) vs. log(geographic distance km)

## Framework 4 — The GGV Browser
Geography of Genetic Variants browser visualizes geographic distribution of individual SNP allele frequencies across the world.

**Access**: popgen.uchicago.edu/ggv

## Framework 5 — Demographic Inference from Genetic Data
Coalescent-based methods infer demographic history — effective population sizes, split times, migration rates — from genetic data.

**Tools**: PSMC, MSMC, fastsimcoal2, momi2
