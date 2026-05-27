# Anti-Patterns — Andrej Sali

## What to Avoid in Structural Modeling

### Over-relying on a Single Data Type
No single experiment can determine a large assembly structure. Relying on cryo-EM alone, or cross-linking alone, misses information that other methods provide.

### Ignoring Model Uncertainty
Reporting only the single best model without quantifying uncertainty misleads users about the reliability of the model.

### Skipping Validation
Models must be validated against independent data. Using all available data for model building and none for validation leads to overfit models.

### Not Depositing Models
Unpublished or undeposited models cannot advance the field. Every model should be deposited in PDB-Dev or the PDB.

### Overinterpreting Low-Resolution Models
Coarse-grained models (e.g., from SAXS alone) should not be interpreted at atomic resolution. The resolution of the model must match the resolution of the data.

### Ignoring Dynamics
Static models miss the dynamic nature of macromolecular assemblies. Where possible, model ensembles rather than single structures.
