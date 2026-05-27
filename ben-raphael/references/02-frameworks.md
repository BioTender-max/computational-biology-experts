# Frameworks — Ben Raphael

## HATCHet Workflow
1. **Input**: Multiple bulk tumor samples from same patient
2. **Allele-specific read counting**: Count reads at heterozygous SNPs
3. **Segmentation**: Identify genomic segments with uniform copy number
4. **Joint optimization**: Infer clone proportions and allele-specific CNAs jointly
5. **WGD detection**: Identify whole-genome duplication events
6. **Output**: Clone-specific copy-number profiles and proportions

## Tumor Evolution Reconstruction
1. **Mutation calling**: Identify somatic mutations in each sample
2. **Clonal decomposition**: Separate mutations into clones
3. **Phylogeny inference**: Reconstruct evolutionary tree of clones
4. **Driver identification**: Identify mutations that drove evolution
5. **Metastasis tracing**: Reconstruct seeding of metastases from primary tumor

## Network/Pathway Analysis
1. **Mutation matrix**: Patients × genes binary mutation matrix
2. **Mutual exclusivity**: Identify mutually exclusive mutation patterns
3. **Co-occurrence**: Identify co-occurring mutations
4. **Pathway enrichment**: Map mutations to biological pathways
5. **Driver pathway identification**: Identify recurrently mutated pathways
