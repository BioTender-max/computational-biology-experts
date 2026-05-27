# Trey Ideker — Analytical Frameworks

## Network Construction Framework
1. Choose interaction type (protein-protein, genetic, co-expression)
2. Collect data (AP-MS, Y2H, E-MAP, RNA-seq)
3. Score interactions (SAINT for AP-MS, ε-score for genetic)
4. Filter by confidence threshold
5. Visualize in Cytoscape
6. Annotate with functional information (GO, pathways)

## Genetic Interaction Analysis Framework
1. Measure single mutant fitness (w_A, w_B)
2. Measure double mutant fitness (w_AB)
3. Compute ε-score: ε = w_AB - w_A × w_B
4. Cluster genes by interaction profile similarity
5. Identify functional modules from clusters
6. Validate with known biology

## Visible Neural Network Framework (DCell/DrugCell)
1. Define biological hierarchy (Gene Ontology, pathway database)
2. Map genes to GO terms (gene annotations)
3. Build VNN: neurons = GO terms, connectivity = GO hierarchy
4. Train on genotype-phenotype data
5. Interpret: which subsystems activate for which mutations?
6. Validate interpretations against known biology

## Cancer Network Medicine Framework
1. Map protein interactions in cancer cell lines (AP-MS)
2. Identify cancer-specific interactions (compare to normal)
3. Map cancer mutations onto interaction network
4. Identify protein complexes disrupted by mutations
5. Predict synthetic lethal partners
6. Validate with CRISPR screens and patient data
