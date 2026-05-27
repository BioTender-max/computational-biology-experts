# John Novembre — Anti-Patterns

## Anti-Pattern 1 — Over-interpreting PCA axes
PCA axes are not always interpretable as geographic directions or historical events. The orientation of the axes depends on sample composition and can change when samples are added or removed. Always interpret PCA carefully.

## Anti-Pattern 2 — Ignoring sample composition effects
The results of PCA depend on which samples are included. Adding or removing populations can change the axes and the apparent clustering. Always consider how sample composition affects your conclusions.

## Anti-Pattern 3 — Confusing genetic distance with geographic distance
Genetic distance and geographic distance are correlated under isolation by distance, but they are not the same. Barriers and corridors can create deviations from this correlation. Use EEMS to model these deviations explicitly.

## Anti-Pattern 4 — Using PCA as a substitute for demographic modeling
PCA reveals structure but doesn't explain it. Understanding the causes of population structure requires demographic modeling (PSMC, MSMC, fastsimcoal). Don't stop at PCA.

## Anti-Pattern 5 — Ignoring ascertainment bias
SNP arrays are ascertained in specific populations (usually European). This can create artifacts in PCA and other analyses when applied to non-European populations. Use whole-genome sequencing or ascertainment-corrected methods when possible.

## Anti-Pattern 6 — Over-fitting demographic models
Demographic models with many parameters can fit the data well without being correct. Use model selection criteria (AIC, BIC) and cross-validation to avoid over-fitting.

## Anti-Pattern 7 — Communicating only to specialists
Population genetics has implications for medicine, anthropology, history, and public policy. Communicate results to broad audiences using clear writing and effective visualization.
