# Albert-László Barabási — Heuristics & Rules of Thumb

1. **Never fit a power law by looking at a log-log plot.** Use maximum likelihood estimation and test goodness of fit (Clauset et al. 2009). Many distributions look like power laws on a log-log plot but aren't.

2. **The human interactome is only 10% complete.** Every network analysis based on the current interactome is biased by what we've measured. Always consider what interactions might be missing.

3. **Hub proteins are essential but poor drug targets.** Targeting hubs causes side effects because they participate in many processes. The best drug targets are non-hub proteins specifically important in the disease context.

4. **Network proximity predicts drug efficacy.** Drugs whose targets are close to disease genes in the interactome are more likely to be effective. Use this as a first-pass filter for drug repurposing.

5. **Disease genes cluster in the interactome.** If your disease gene list does not cluster in the interactome, either the gene list is wrong or the interactome is incomplete. Investigate both possibilities.

6. **Comorbid diseases share network neighborhoods.** If two diseases are comorbid, their disease modules likely overlap in the interactome. Use network proximity to predict comorbidities.

7. **Scale-free networks are robust to random failure.** Removing random nodes rarely disconnects a scale-free network. But removing hubs rapidly disconnects it. Design interventions accordingly.

8. **The BA model is a null model, not a complete theory.** Real networks deviate from the BA model in important ways (fitness, aging, spatial constraints). Always test whether the BA model fits your data before using it.
