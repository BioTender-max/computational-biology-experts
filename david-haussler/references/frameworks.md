# Frameworks — David Haussler

Named, repeatable procedures with steps and application conditions.

---

## 1. The Comparative Genomics Decoding Pipeline

**When to apply**: Identifying functional elements in a newly sequenced genome,
or prioritizing regions for experimental follow-up.

**Steps**:
1. Align the target genome to a phylogenetically diverse set of reference genomes
   (vertebrates, invertebrates, plants as appropriate)
2. Compute conservation scores using phylogenetic HMMs (phastCons for elements,
   phyloP for per-base scores)
3. Identify regions under negative selection (conserved = functional)
4. Scan for lineage-specific accelerated change (positive selection signal)
5. Intersect with known gene annotations, regulatory elements, and ENCODE data
6. Rank candidates by conservation depth × lineage specificity
7. Prioritize for experimental validation; ignore non-conserved regions unless
   there is a specific hypothesis

**Source**: Haussler (2003) ACM STOC; Pollard et al. (2006) Nature; Siepel &
Haussler (2003, 2005)

---

## 2. The HMM Unification Framework

**When to apply**: When multiple ad hoc methods exist for the same sequence
analysis problem and you need a principled, scalable solution.

**Steps**:
1. Identify the underlying probabilistic structure (states = biological features,
   transitions = grammar of valid sequences, emissions = nucleotide/amino acid
   probabilities)
2. Define a generalized HMM (GHMM) that encodes the grammar of valid sequences
3. Estimate parameters from a training corpus using dynamic programming
   (Viterbi for decoding, Baum-Welch for parameter estimation)
4. Validate on held-out data with sensitivity/specificity metrics
5. Extend by combining with discriminative methods (SVMs via Fisher kernel)
   for improved classification of remote homologs
6. Scale: HMMs are linear in data size, so exponential data growth gives
   exponential leverage

**Source**: Krogh et al. (1994) NAR; Kulp et al. (1996) ISMB; Jaakkola &
Haussler (1998); Siepel & Haussler (2003)

---

## 3. The Pangenome Reference Construction Workflow

**When to apply**: Building or using a population-representative genomic reference
that captures human diversity.

**Steps**:
1. Assemble diverse, phased diploid genomes using long-read sequencing (HiFi + Hi-C)
   from individuals representing global genetic diversity
2. Quality-control assemblies (>99% sequence coverage, >99% base accuracy)
3. Align assemblies using graph-based tools (Minigraph-Cactus)
4. Construct a variation graph encoding all haplotypes as paths through shared nodes
5. Annotate the graph with functional elements, gene models, and population
   frequencies
6. Validate: structural variant detection should improve >100% vs. linear reference;
   small variant errors should decrease >30%
7. Distribute via open standards (GA4GH DRS, VCF, GFA) with unrestricted access

**Source**: Human Pangenome Reference Consortium (2023) Nature; Human Pangenome
Project (2022) Nature

---

## 4. The Open Data Infrastructure Stack

**When to apply**: Designing systems for sharing genomic data across institutions
and jurisdictions while respecting consent and privacy.

**Steps**:
1. Separate data storage from data access (federated model: data stays at the
   institution, APIs enable remote access)
2. Implement standard APIs (GA4GH DRS for data retrieval, Beacon for variant
   discovery, htsget for streaming) for interoperability
3. Use consent frameworks that allow secondary research use (broad consent)
4. Build visualization layers (UCSC Browser, Xena) that work across federated hubs
5. Ensure all reference data is freely downloadable without registration
6. Engage international partners (H3Africa, NCIG) to ensure global representation

**Source**: GA4GH founding; UCSC Xena (Goldman et al. 2018, 2019, 2021);
UCSC Genome Browser (Kent et al. 2002)

---

## 5. The Skunk-Works Crisis Response

**When to apply**: When a critical bottleneck threatens a field-defining project
and no one else is solving it.

**Steps**:
1. Identify the single blocking problem (e.g., genome assembly failing in 2000)
2. Find the one person with the right combination of skills and temperament
   (deep technical skill + ability to hold all complexity in one mind)
3. Give them full autonomy and remove all bureaucratic friction
4. Set a hard deadline tied to an external forcing function
5. Provide support (resources, moral backing) but not interference
6. Accept that a committee cannot do what one genius can do in four weeks

**Source**: PLOS Genetics interview (2013) — account of Jim Kent's genome assembly
