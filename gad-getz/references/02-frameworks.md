# Frameworks — Gad Getz

## MutSig Workflow
1. **Input**: Somatic mutation calls from tumor-normal pairs
2. **Background model**: Estimate background mutation rate per gene (sequence context, expression, replication timing)
3. **Statistical test**: Compare observed mutation rate to background
4. **Multiple testing correction**: FDR correction across all genes
5. **Output**: Significantly mutated genes (SMGs)

## MuTect Workflow
1. **Input**: Tumor and matched normal BAM files
2. **Candidate site identification**: Sites with evidence of somatic mutation
3. **Bayesian model**: Compute posterior probability of somatic mutation
4. **Filtering**: Remove germline variants, sequencing artifacts
5. **Output**: High-confidence somatic SNVs

## GISTIC Workflow
1. **Input**: Copy-number profiles across tumor cohort
2. **Segmentation**: Identify copy-number segments
3. **Significance testing**: Identify recurrently amplified/deleted regions
4. **Output**: Significantly amplified/deleted regions (cancer drivers)
