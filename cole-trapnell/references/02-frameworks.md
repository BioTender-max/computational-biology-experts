# Cole Trapnell — Analytical Frameworks

## Monocle 3 Trajectory Analysis
1. Preprocess data (PCA, UMAP)
2. Cluster cells
3. Learn principal graph on UMAP embedding
4. Select root cells (earliest time point)
5. Order cells by pseudotime (geodesic distance from root)
6. Find trajectory-dependent genes (graph_test)

## sci-RNA-seq Experimental Framework
1. Fix cells with formaldehyde
2. Round 1 barcoding (RT primer in 96-well plate)
3. Pool and redistribute
4. Round 2 barcoding (ligation adapter)
5. Optional Round 3 barcoding
6. Sequence and demultiplex

## Differential Abundance Framework (Milo)
1. Build k-nearest neighbor graph
2. Define neighborhoods around each cell
3. Test each neighborhood for differential abundance (negative binomial GLM)
4. Identify cell states that change in abundance between conditions
