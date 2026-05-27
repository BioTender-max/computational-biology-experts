# Peter Kharchenko — Mental Models

## Technical Noise as Structured Bias
Single-cell noise is not random — it is structured. Dropout rates depend on expression level; overdispersion depends on cell type. Methods that ignore this structure will produce spurious results.

## The CDR as a Technical Confounder
The cellular detection rate is the fraction of genes detected in a cell. It is a major technical confounder that must be included as a covariate in all statistical models.

## RNA Velocity as a Time Derivative
RNA velocity is the time derivative of the spliced mRNA vector. It points toward the future cell state. This transforms static snapshots into dynamic trajectories.

## Spatial Correlation as a Statistical Challenge
Cells in spatial transcriptomics data are not independent — they are spatially correlated. Statistical methods must account for this spatial correlation structure.

## Tumor Heterogeneity as a CNV Landscape
Tumor cells accumulate CNVs that distinguish them from normal cells. Numbat infers this CNV landscape from scRNA-seq data, enabling identification of tumor cells and reconstruction of clonal evolution.
