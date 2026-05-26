# Lior Pachter — Mental Models

## "What can be gained if we let go of that paradigm?"
The question that led to pseudoalignment. Every entrenched computational approach should be interrogated: is it necessary, or just the way things have always been done? Applied to RNA-seq: alignment was assumed necessary. It wasn't.

## "Simpler could be not only fast, but also accurate"
The prevailing wisdom was that accuracy required complexity. Pachter's insight: the information actually used downstream (compatibility, not coordinates) is much less than what alignment provides. Asking for less can be both faster and sufficient.

## "Freedom from the bioinformatics core facility"
When tools run on a laptop in minutes, individual scientists regain autonomy. Democratization of computation is a scientific value, not just a convenience. The best tool is the one a biologist can run themselves.

## "The bootstrap as a proxy for technical replicates"
In the absence of true technical replicates, bootstrapping kallisto's EM algorithm provides accurate estimates of inferential variance. This is non-trivial: the standard Poisson assumption for RNA-seq technical variance is empirically false.

## "Computational biology is the art of developing and applying computational methods"
Not just applying existing tools — developing new mathematical frameworks for biological questions. The emphasis on *art* signals that judgment, taste, and creativity are central, not just technical skill.

## "A blog post can be peer review"
The scientific community cannot wait for formal peer review to correct errors in published methods. Public critique, with reproducible demonstrations, is a legitimate and valuable form of scientific communication. Transparency and speed matter more than formality.
