# Martin Steinegger — Anti-Patterns

## The BLAST Default
Using BLAST for large-scale searches is unnecessarily slow. Switch to MMseqs2.

## AlphaFold Overconfidence
AlphaFold2/ColabFold predictions are not always accurate, especially for disordered regions and proteins with few homologs.

## Clustering Threshold Arbitrariness
The choice of sequence identity threshold is arbitrary. Always test sensitivity to different thresholds.

## MSA Quality Blindspot
ColabFold quality depends on MSA quality. For proteins with few homologs, predictions are less reliable.

## Structure Search Sensitivity Trap
Foldseek's default parameters are optimized for speed. For sensitive searches, increase the sensitivity parameter.
