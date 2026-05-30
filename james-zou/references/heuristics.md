## Key heuristics

- Always compute SHAP values for any clinical ML model. If the top
  features don't make biological sense, the model has learned a spurious
  correlation.
- Validate AI models on data from different hospitals, time periods, and
  patient populations before clinical deployment. Distribution shift is
  the most common failure mode.
- When using real-world data, explicitly model the selection bias in
  what gets recorded. Missing data is not random in EHRs.
- For foundation model interpretability, start with probing classifiers
  on known biological concepts before using SAEs for discovery.
- Design virtual lab agents with specialized roles and explicit
  disagreement protocols. Homogeneous agents produce groupthink.

---