# Mental Models — Núria López-Bigas

## 1. The Needle-in-a-Haystack Problem

Of the thousands of mutations in a tumor, only 2–4 are drivers. Finding them requires not just looking harder, but looking smarter — using the right statistical framework (positive selection), the right scale (thousands of tumors), and the right combination of signals.

The haystack is not random; it has structure (chromatin, replication timing, sequence context) that must be modeled to find the needle. A naive search (looking for the most mutated genes) will find the wrong needles — genes that are mutated frequently because they are large or in high-mutation-rate regions, not because they are drivers.

**Application**: Before building a driver detection method, ask: what is the structure of the haystack? What determines the background mutation rate? Only after modeling the haystack can you reliably identify the needle.

---

## 2. Tumors as Replicated Natural Experiments

Each patient's tumor is an independent experiment testing the oncogenic potential of its mutations. Across thousands of patients, the same driver mutations recur because they confer the same selective advantage. This replication is the statistical foundation of driver detection: what is selected for will appear more often than chance predicts.

This mental model reframes the role of large tumor cohorts: they are not just bigger datasets, they are more replicates of the same experiment. Each additional tumor increases the statistical power to detect the signal of positive selection.

**Application**: When designing a study, think about how many independent replicates (tumors) you need to detect the effect size you expect. For rare drivers, you need very large cohorts.

---

## 3. The Mutation Rate Landscape as Terrain

The genome is not a flat surface for mutation accumulation. It is a terrain shaped by chromatin organization, replication timing, transcription factor binding, and nucleosome positioning. Some regions are mutation deserts (early-replicating, open chromatin, actively repaired by NER); others are mutation mountains (late-replicating, heterochromatic, poorly repaired).

Understanding this terrain is prerequisite to identifying the peaks that represent true driver hotspots rather than high-mutation-rate artifacts. The 10-bp periodicity of mutation rates around nucleosomes, and the elevated mutation rates at transcription factor binding sites (due to NER impairment), are features of this terrain.

**Application**: When interpreting mutation hotspots, always ask: is this hotspot elevated above the local terrain, or is it just in a high-altitude region? The terrain must be subtracted before the signal can be interpreted.

---

## 4. The VUS Interpretation Bottleneck

Tumor sequencing generates thousands of variants; most are of uncertain significance. The bottleneck in precision oncology is not sequencing — it is interpretation. Every tool López-Bigas builds (IntOGen, BoostDM, CGI) is designed to attack this bottleneck: converting VUS into actionable classifications that guide treatment decisions.

This mental model clarifies the research agenda: the scientific problem is not generating more data, it is building better interpretation tools. The data is already outpacing our ability to interpret it.

**Application**: When evaluating the clinical utility of a new sequencing technology, ask: do we have the interpretation tools to make use of the additional data? If not, the bottleneck is interpretation, not sequencing.

---

## 5. Cancer as a Continuous Darwinian Process

Cancer does not happen in a day. It is a gradual process of variation (random mutation) and selection (proliferative advantage) operating over years or decades. By the time a tumor is diagnosed, the cells have a long evolutionary history. Early-stage clonal expansions in healthy tissue (clonal hematopoiesis, field cancerization) are part of the same continuum.

This temporal dimension means that the tumor genome at diagnosis is a snapshot of an ongoing evolutionary process, not a static object. The mutations present reflect the history of selection, not just the current state.

**Application**: When interpreting a tumor genome, think about the evolutionary trajectory that produced it. Which mutations were early (likely drivers that initiated the clone) and which were late (likely passengers or secondary drivers)? Clonal architecture analysis can reconstruct this history.

---

## 6. The Data-Interpretation Flywheel

"It's like a fish that eats its tail: the more data we have, the more information we can extract that helps us better interpret the next patient." Each new tumor genome adds to the training data for models, improves background estimates, and refines driver classifications. The system is self-improving.

This flywheel has a minimum viable scale: below a certain number of tumors, the models are too noisy to be useful. Above that threshold, each additional tumor improves the models for all future patients. This creates a strong argument for data sharing and large-scale consortia.

**Application**: When building machine learning models for clinical genomics, design for continuous learning. Build infrastructure that allows models to be retrained as new data accumulates. The model you deploy today should be better than the model you deployed last year.
