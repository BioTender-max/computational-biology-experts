# Martin Steinegger — Analytical Frameworks

## MMseqs2 Sequence Analysis Framework
1. Create MMseqs2 database from FASTA file
2. Search query sequences against target database
3. Filter results by e-value and identity threshold
4. Convert results to BLAST-like format
5. Downstream analysis (functional annotation, phylogenetics)

## ColabFold Structure Prediction Framework
1. Input protein sequence(s)
2. Fast MSA generation (MMseqs2 against ColabFold server)
3. AlphaFold2 structure prediction
4. Optional: AMBER relaxation
5. Evaluate prediction quality (pLDDT, PAE)
6. Validate key predictions experimentally

## Foldseek Structure Search Framework
1. Create Foldseek database from PDB/AlphaFold structures
2. Search query structure against database
3. Filter by probability and e-value
4. Align query and target structures
5. Identify structural homologs
6. Infer function from structural homologs

## Linclust Clustering Framework
1. Create MMseqs2 database
2. Run Linclust with desired identity threshold
3. Extract representative sequences
4. Annotate representatives
5. Map all sequences to representatives
