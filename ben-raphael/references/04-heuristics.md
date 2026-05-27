# Heuristics — Ben Raphael

## Practical Rules for Algorithmic Cancer Genomics

1. **Use multi-sample analysis**: Single samples miss the clonal architecture; always analyze multiple samples when available.

2. **Use allele-specific copy number**: Copy-number analysis without allele resolution misses important evolutionary events.

3. **Validate algorithms on simulated data**: Before applying to real data, validate algorithms on simulated data with known ground truth.

4. **Use matched normals**: Somatic mutation calling requires matched normal tissue to distinguish somatic from germline variants.

5. **Consider whole-genome duplication**: WGD is common in cancer and profoundly affects copy-number interpretation.

6. **Integrate multiple data types**: Combining SNV, CNA, and SV data provides a more complete picture of tumor evolution.
