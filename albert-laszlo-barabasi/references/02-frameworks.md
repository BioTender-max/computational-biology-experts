# Albert-László Barabási — Analytical Frameworks

## Scale-Free Network Analysis Framework
1. Measure degree distribution P(k)
2. Test for power law using MLE + KS goodness-of-fit test (not log-log plot)
3. Estimate exponent γ and minimum degree k_min
4. Identify hubs (top 1% by degree)
5. Analyze hub properties (essentiality, conservation, disease association)
6. Test robustness to random failure vs. targeted attack

## Disease Module Framework
1. Collect disease gene list (OMIM, GWAS, literature)
2. Map disease genes onto interactome
3. Identify disease module using DIAMOnD algorithm
4. Compute disease-disease separation scores
5. Identify overlapping disease modules (shared mechanisms, comorbidities)
6. Validate module with functional experiments

## Drug Repurposing via Network Proximity
1. Map drug targets onto interactome
2. Map disease genes onto interactome
3. Compute network proximity (closest, symmetric, or kernel-based)
4. Compute z-score relative to random permutations
5. Prioritize drugs with z < -1.5 (close to disease module)
6. Validate top predictions experimentally

## Network Controllability Framework
1. Build directed network (regulatory, signaling)
2. Find minimum dominating set (driver nodes)
3. Identify which nodes are driver nodes
4. Analyze driver node properties (degree, essentiality, druggability)
5. Design intervention strategy targeting driver nodes
