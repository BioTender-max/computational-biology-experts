# Heuristics — Gunnar Rätsch

## Practical Rules for ML in Biomedicine

1. **Design for clinical use**: Always ask whether a model can be used by clinicians. If not, it has limited value.

2. **Prioritize interpretability**: For clinical applications, interpretable models are more valuable than black-box models.

3. **Validate on independent cohorts**: Clinical ML models must be validated on data from different institutions and time periods.

4. **Use spatial context in pathology**: H&E images contain spatial information; models that ignore it miss important biology.

5. **Collaborate with clinicians**: Computational methods developed without clinical input often fail to address real clinical problems.

6. **Integrate multiple data types**: No single data type captures the full complexity of cancer; integration is essential.
