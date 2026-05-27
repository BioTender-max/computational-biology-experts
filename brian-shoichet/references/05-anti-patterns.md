# Anti-Patterns — Brian Shoichet

## What to Avoid in Computational Drug Discovery

### Ignoring Aggregation
Many "hits" in biochemical screens are artifacts of colloidal aggregation. Always test with detergent before concluding that a compound is a true inhibitor.

### Docking Without Experimental Validation
Computational predictions must be tested; docking scores are not binding affinities. Reporting docking results without experimental validation is misleading.

### Ignoring Protein Flexibility
Rigid docking misses many true binders. Induced fit and conformational selection are important for many drug targets.

### Overinterpreting Selectivity
Most ligands bind multiple targets. Always profile against related proteins before claiming selectivity.

### Using Low-Quality Protein Structures
Docking quality depends critically on structure quality. Using low-resolution or poorly refined structures leads to poor predictions.

### Ignoring Physicochemical Properties
Compounds that bind in silico may not be drug-like. Always consider solubility, permeability, and metabolic stability.
