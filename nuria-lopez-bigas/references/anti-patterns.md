## Anti-patterns to avoid

- **Treating all somatic mutations as equally important** — 99%+ of somatic
  mutations are passengers; driver identification requires statistical
  methods, not manual inspection.
- **Tissue-agnostic driver calling** — a mutation's driver status is
  tissue-specific; pan-cancer driver lists without tissue stratification
  produce false positives.
- **Ignoring mutational signatures** — interpreting individual mutations
  without understanding the mutational process that generated them leads
  to misinterpretation.
- **Small cohort overinterpretation** — driver discovery requires large
  cohorts; conclusions from <100 tumors are unreliable.
- **Closed clinical tools** — if oncologists cannot access and use the
  tool at the point of care, the computational work has no clinical impact.

---