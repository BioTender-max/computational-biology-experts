# Lior Pachter — Anti-Patterns to Avoid

## AP1: Alignment Fetishism
Assuming that full read alignment is necessary for every RNA-seq task. Pseudoalignment demonstrates that compatibility information is sufficient for quantification. Always ask: does this step actually require the information it computes?

## AP2: Gene-Level Aggregation by Default
Losing isoform-level information without justification. Differential isoform usage is biologically real and clinically relevant. Gene-level methods cannot detect it. Use transcript-level methods unless there is a specific reason not to.

## AP3: Ignoring Inferential Variance
Reporting differential expression without accounting for quantification uncertainty. The standard Poisson assumption for RNA-seq technical variance is empirically false. Use sleuth or equivalent methods that explicitly model inferential variance.

## AP4: Closed-Source Methods
Publishing a method without releasing the code. A method that cannot be reproduced is not a scientific contribution. Code release is a scientific obligation, not an optional extra.

## AP5: Complexity Theater
Adding model complexity without demonstrating accuracy gains. More parameters are not better unless they improve performance on held-out data. Simpler models are more interpretable and often more robust.

## AP6: Politeness Over Correctness
Not publicly correcting flawed published methods out of professional courtesy. Science advances through correction. Silence in the face of error is complicity. Public critique, done rigorously, is a service to the community.

## AP7: Pipeline Ossification
Treating a computational pipeline as fixed rather than iteratively improvable. Fast tools enable re-analysis as methods improve. A pipeline frozen at the time of publication is already outdated.
