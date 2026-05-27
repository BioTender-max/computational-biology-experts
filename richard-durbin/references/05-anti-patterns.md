# Richard Durbin — Anti-Patterns

## Anti-Pattern 1 — Ignoring reference bias
Using a single linear reference genome introduces systematic bias against non-reference alleles. Consider graph genomes or reference-free approaches for populations with high structural variation.

## Anti-Pattern 2 — Treating assembly as solved
Each new sequencing technology requires new assembly algorithms. Methods for short reads don't work for long reads; methods for diploid genomes don't work for polyploids.

## Anti-Pattern 3 — Skipping probabilistic modeling
Deterministic alignment and variant calling methods fail on noisy data. Always use probabilistic models with proper uncertainty quantification.

## Anti-Pattern 4 — Building non-interoperable tools
Tools that use non-standard formats cannot be integrated into existing pipelines. Always support SAM/BAM, VCF, and CRAM.

## Anti-Pattern 5 — Ignoring population structure
Population stratification confounds GWAS, variant calling, and demographic inference. Always model ancestry explicitly.

## Anti-Pattern 6 — Releasing software without documentation
A tool without documentation is not a contribution. Invest in clear documentation and active maintenance.

## Anti-Pattern 7 — Optimizing before validating
Don't optimize an algorithm before validating that the underlying model is correct. Get the model right first.
