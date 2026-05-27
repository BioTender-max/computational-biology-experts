# Peter Kharchenko — Anti-Patterns

## Zero-Inflation Blindspot
Treating all zeros as true zeros ignores dropout events. Use SCDE or similar methods.

## CDR Confounding
Failing to account for CDR leads to spurious correlations between genes.

## Velocity Overinterpretation
RNA velocity arrows show direction of transcriptional change, not actual cell trajectories.

## CNV False Positive
CNV inference can produce false positives due to allele-specific expression. Validate with WGS.

## Spatial Segmentation Error
Poor cell segmentation leads to contamination of cell profiles with neighboring cell transcripts.
