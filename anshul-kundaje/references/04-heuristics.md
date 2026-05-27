# Heuristics — Anshul Kundaje

## Practical Rules for Deep Learning in Regulatory Genomics

1. **Use base-pair resolution**: Peak-level models miss the fine-grained regulatory logic; base-pair resolution is where the biology lives.

2. **Always interpret your models**: Use TF-MoDISco or similar tools to extract biological insight from deep learning models.

3. **Use ENCODE pipelines for data processing**: Uniform processing is essential for reproducibility and comparability.

4. **Validate on held-out cell types**: Models must generalize to cell types not seen during training.

5. **Score variants in context**: Variant effects depend on the surrounding sequence context; always score variants in their genomic context.

6. **Combine with genetic data**: Regulatory models are most powerful when combined with GWAS and eQTL data to identify disease-relevant variants.
