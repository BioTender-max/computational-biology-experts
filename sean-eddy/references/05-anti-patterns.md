# Sean Eddy — Anti-Patterns

## Anti-Pattern 1 — Using BLAST for sensitive homology detection
BLAST uses heuristic scoring and is not statistically optimal. For detecting remote homologs (< 30% identity), HMMER is significantly more sensitive. Using BLAST alone will miss many true homologs.

## Anti-Pattern 2 — Reporting percent identity as a homology measure
Percent identity is not statistically calibrated — a 25% identity hit may be significant or not depending on alignment length and amino acid composition. Always use E-values.

## Anti-Pattern 3 — Ignoring noncoding RNA
Annotating a genome without searching for noncoding RNAs misses a major functional component. Always run Infernal against Rfam as part of genome annotation.

## Anti-Pattern 4 — Using Viterbi scores for database search
Viterbi finds the best single alignment; forward sums over all alignments. For database search, forward scores are more sensitive. HMMER3 uses forward by default — don't override this.

## Anti-Pattern 5 — Trusting uncalibrated E-values
Many tools report "E-values" that are not properly calibrated against random sequence distributions. HMMER's E-values are calibrated; treat other tools' E-values with skepticism.

## Anti-Pattern 6 — Building profiles from unaligned sequences
Profile HMMs must be built from multiple sequence alignments. Building from unaligned sequences produces a poor model. Always align first, then build.

## Anti-Pattern 7 — Ignoring the gathering threshold
Pfam and Rfam families have curated gathering thresholds (--cut_ga) that define the boundary between true and false positives. Using arbitrary E-value cutoffs instead of gathering thresholds leads to inconsistent annotation.
