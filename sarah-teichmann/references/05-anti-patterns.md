# Sarah Teichmann — Anti-Patterns

## Dissociation Artifact
Genes induced by dissociation stress (HSP70, FOS, JUN) will appear differentially expressed if not corrected.

## Doublet Contamination
Droplet-based methods capture doublets (~1% per 1,000 cells). Use DoubletFinder or Scrublet.

## Ambient RNA Problem
Ambient RNA from lysed cells contaminates all droplets. Use SoupX or CellBender.

## Tissue-Specific Bias
Rare cell types are underrepresented. Use enrichment strategies for rare cell types.

## Cross-Tissue Comparison Pitfall
The same cell type (e.g., macrophages) has different gene expression in different tissues. Careful normalization is required.
