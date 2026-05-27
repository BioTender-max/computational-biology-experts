# Peter Kharchenko — Heuristics

1. Model dropout explicitly — methods that treat zeros as true zeros produce spurious results.
2. Include CDR as a covariate in all differential expression models.
3. Use PAGODA for pathway-level analysis of cell-to-cell heterogeneity.
4. Validate RNA velocity directions against known developmental trajectories.
5. Use Numbat for tumor heterogeneity — CNV inference without separate WGS.
6. Use Baysor for imaging-based spatial data — better segmentation than watershed.
7. Use Conos for multi-dataset integration without batch correction.
8. Validate CNV calls with orthogonal methods (WGS, FISH).
