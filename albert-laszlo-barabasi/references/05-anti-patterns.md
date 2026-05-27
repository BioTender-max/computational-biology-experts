# Albert-László Barabási — Anti-Patterns to Avoid

## The Power Law Everywhere Fallacy
Not every heavy-tailed distribution is a power law. Many distributions (log-normal, stretched exponential) look like power laws on a log-log plot but have different statistical properties. Always test goodness of fit rigorously.

## The Static Network Mistake
Real biological networks are dynamic — interactions change with cell type, developmental stage, and environmental condition. Analyzing a static snapshot misses context-dependence.

## The Guilt-by-Association Overreach
Network proximity predicts biological relationships, but proximity alone is not sufficient evidence for a causal relationship. A gene close to disease genes in the interactome is a candidate, not a confirmed disease gene.

## The Hub Targeting Trap
Targeting hub proteins is tempting because they have large network effects. But hub proteins are often essential in normal cells, leading to toxicity. The best drug targets are often non-hub proteins specifically important in the disease context.

## The Interactome Incompleteness Bias
Current interactome maps are biased toward well-studied proteins. This "study bias" can confound network analyses. Always consider whether results could be explained by study bias.

## The Network Visualization Trap
A beautiful network visualization is not a scientific result. Visualizations can be misleading if the layout algorithm introduces spurious patterns. Always report quantitative network statistics.

## The Preferential Attachment Universality Claim
Not all networks grow by preferential attachment. Some networks are designed (regulatory networks), some are constrained by physics (metabolic networks), and some grow by different mechanisms. Always test whether preferential attachment explains your network's degree distribution.
