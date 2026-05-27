# Trey Ideker — Heuristics & Rules of Thumb

1. **Visualize networks in Cytoscape first.** Before any analysis, visualize the network. Visual inspection reveals structure that statistics miss.

2. **Filter to the relevant subnetwork.** Never analyze the full interactome — filter to disease-relevant genes, differentially expressed genes, or mutated genes before analysis.

3. **Validate synthetic lethal predictions with CRISPR screens.** Computational synthetic lethality predictions have high false positive rates. Always validate with combinatorial CRISPR screens before clinical translation.

4. **Use multiple interaction data types.** Protein interactions tell you who talks to whom; genetic interactions tell you who needs whom; expression data tells you who is active. Integrate all three.

5. **Check VNN interpretations against known biology.** If the DNA repair subsystem doesn't activate when DNA repair genes are mutated, something is wrong with the model.

6. **Report network statistics, not just visualizations.** A beautiful network visualization is not a scientific result. Always report quantitative statistics (degree distribution, clustering coefficient, modularity).

7. **Consider network context when interpreting mutations.** The same mutation can have different effects in different network contexts. Always analyze mutations in the context of the full network.

8. **Build tools that others can use.** The most impactful contribution is a tool that thousands of scientists use. Invest in usability, documentation, and community building.
