# Frameworks — Brian Shoichet

## Structure-Based Drug Discovery Pipeline
1. **Target selection**: Choose a protein with known structure and therapeutic relevance
2. **Library preparation**: Prepare virtual library (ZINC database, billions of compounds)
3. **Docking**: Screen library against protein structure using DOCK
4. **Scoring**: Rank compounds by predicted binding affinity
5. **Selection**: Choose top-ranked compounds for experimental testing
6. **Experimental validation**: Test binding (ITC, SPR), activity (biochemical assay), and structure (X-ray crystallography)
7. **Iteration**: Use experimental results to improve docking and select next round

## Aggregation Detection Protocol
1. Run biochemical assay at multiple compound concentrations
2. Add detergent (0.01% Triton X-100) and repeat
3. If inhibition disappears with detergent → aggregation artifact
4. If inhibition persists → likely real inhibition
5. Confirm with dynamic light scattering (DLS)

## SEA (Similarity Ensemble Approach)
1. Represent each drug as a set of known ligands
2. Compare ligand sets between drugs and targets
3. Identify unexpected similarities → predict new targets
4. Validate experimentally
