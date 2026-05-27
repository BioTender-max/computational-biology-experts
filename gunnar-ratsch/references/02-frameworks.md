# Frameworks — Gunnar Rätsch

## Tumor Profiler Workflow
1. **Patient enrollment**: Biopsy from cancer patient
2. **Multi-omics profiling**: WGS, RNA-seq, proteomics, imaging
3. **ML analysis**: Integrate all data types
4. **Treatment recommendation**: ML-guided treatment selection
5. **Clinical validation**: Track patient outcomes
6. **Model improvement**: Use outcomes to improve models

## Deep Learning for Pathology
1. **Input**: H&E stained tissue images
2. **Preprocessing**: Tile extraction, normalization
3. **Model**: CNN with spatial attention
4. **Training**: Predict molecular subtypes, survival, treatment response
5. **Interpretation**: Attention maps reveal predictive regions
6. **Validation**: Independent cohort validation

## Clinical NLP Pipeline
1. **Input**: Electronic health records (free text)
2. **NLP**: Named entity recognition, relation extraction
3. **Structured data**: Extract clinical variables
4. **Analysis**: Statistical or ML analysis of extracted data
5. **Output**: Clinical insights from unstructured text
