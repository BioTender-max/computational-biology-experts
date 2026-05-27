# Frameworks — Wouter Meuleman

## DHS Index Construction
1. **DNase-seq data**: Collect DNase I hypersensitivity data across 700+ biosamples
2. **Peak calling**: Identify open chromatin regions in each biosample
3. **Index construction**: Create a non-redundant index of all DHS sites
4. **Annotation**: Annotate each DHS with cell-type activity patterns
5. **Variant interpretation**: Use DHS index to interpret non-coding variants

## DNA-Diffusion Workflow
1. **Training data**: scATAC-seq peaks across cell types
2. **Diffusion model**: Train generative model on regulatory sequences
3. **Conditioning**: Condition on desired cell-type accessibility profile
4. **Generation**: Generate synthetic regulatory sequences
5. **Validation**: Test generated sequences in reporter assays
