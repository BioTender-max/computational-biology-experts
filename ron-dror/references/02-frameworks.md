# Frameworks — Ron Dror

## Bottom-Up (Physics-Based) Approach
1. Define atomic force field (CHARMM, AMBER, etc.)
2. Set up simulation system (protein + ligand + water + ions)
3. Run molecular dynamics simulation
4. Analyze trajectories for binding events, conformational changes
5. Extract mechanistic insights

## Top-Down (Data-Driven) Approach
1. Collect experimental data (cryo-EM, NMR, biochemical)
2. Train ML model to infer structural models from data
3. Validate predictions against held-out data
4. Interpret model to extract biological insights

## GPCR Drug Discovery Pipeline
1. Obtain GPCR crystal structure (with collaborators like Kobilka)
2. Run MD simulations to explore conformational landscape
3. Identify binding sites and allosteric pockets
4. Use ML to predict ligand binding affinities
5. Validate with experimental binding assays
