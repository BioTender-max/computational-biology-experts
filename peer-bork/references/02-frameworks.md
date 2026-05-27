# Peer Bork — Analytical Frameworks

## STRING Protein Network Analysis
1. Query STRING for protein interactions (web or API)
2. Filter by confidence score (>400 for medium confidence; >700 for high)
3. Identify network modules (clusters of interacting proteins)
4. Functional enrichment of modules (GO, KEGG)
5. Identify hub proteins (high degree nodes)
6. Validate key interactions experimentally

## Enterotype Analysis Framework
1. Compute genus-level abundance table
2. Calculate Jensen-Shannon divergence distance matrix
3. Partition around medoids (PAM) clustering
4. Determine optimal k (Calinski-Harabasz index)
5. Assign enterotype labels
6. Associate enterotypes with metadata (diet, health status)

## Comparative Metagenomics Framework
1. Collect samples from diverse environments
2. Shotgun metagenomics sequencing
3. Assembly and gene prediction (MOCAT2)
4. Taxonomic profiling (mOTU)
5. Functional profiling (eggNOG)
6. Comparative analysis across environments
