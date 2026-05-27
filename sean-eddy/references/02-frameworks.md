# Sean Eddy — Conceptual Frameworks

## Framework 1 — Profile Hidden Markov Models
A profile HMM represents a protein family as a probabilistic model with match states (position-specific amino acid frequencies), insert states (background frequencies), and delete states. Trained on a multiple sequence alignment; used to score new sequences via the forward algorithm.

**Tools**: HMMER (hmmbuild, hmmsearch, hmmscan), Pfam database

## Framework 2 — Covariance Models for RNA
RNA secondary structure is conserved even when sequence is not. Covariance models extend profile HMMs with a stochastic context-free grammar modeling base-pair correlations. Enables detection of RNA families at much greater evolutionary distances than sequence-only methods.

**Tools**: Infernal (cmbuild, cmsearch, cmpress, cmscan), Rfam database

## Framework 3 — The Forward Algorithm vs. Viterbi
Viterbi finds the single most probable path (best alignment). Forward sums over all possible paths (all alignments). For homology detection, forward is more sensitive. HMMER3 uses forward for scoring.

## Framework 4 — Extreme Value Distribution Theory
Maximum scores from random sequence searches follow a Gumbel distribution. HMMER calibrates E-values by fitting this distribution to random sequence searches, giving statistically rigorous significance estimates.

## Framework 5 — The Rfam Database
Rfam catalogs RNA families, each represented by a covariance model, seed alignment, and consensus secondary structure. Covers riboswitches, ribozymes, snoRNAs, miRNAs, lncRNAs.

**Access**: rfam.xfam.org; use Infernal for searching
