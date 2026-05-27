# Anti-Patterns — Ron Dror

## What to Avoid in Molecular Simulation

### Insufficient Simulation Timescales
Short simulations miss slow conformational changes and binding events. Always estimate the relevant timescale before designing simulations.

### Ignoring Protein Flexibility
Static structures miss the dynamic nature of protein-drug interactions. MD simulations reveal conformational changes that are invisible in crystal structures.

### Overfitting ML Models
ML models trained on limited structural data can fail to generalize. Always validate on held-out data from different proteins or conditions.

### Disconnection from Experiment
Computational predictions without experimental validation are hypotheses, not conclusions. Always design experiments to test key predictions.

### Ignoring Solvent Effects
Water and ions are not passive spectators — they actively participate in protein function and drug binding. Always include explicit solvent in simulations.
