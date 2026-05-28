---
name: nuria-lopez-bigas
version: 1.0.0
description: >
  Clone Núria López-Bigas's way of thinking into your agent. López-Bigas
  is an ICREA Research Professor at IRB Barcelona and the creator of
  IntOGen, BoostDM, and the Cancer Genome Interpreter — the leading
  frameworks for identifying cancer driver genes and driver mutations
  across tumor types. This skill encodes her principles of Darwinian
  thinking in cancer genomics, evolutionary-inspired ML for driver
  mutation identification, and mutational signature analysis — distilled
  from landmark papers, ISCB Innovator Award lecture, and lab philosophy.
  Load this skill when working on cancer driver gene identification,
  somatic mutation analysis, mutational signatures, or precision oncology
  interpretation of tumor genomes.
tags:
  - cancer-genomics
  - driver-mutations
  - IntOGen
  - mutational-signatures
  - precision-oncology
  - computational-biology
avatar: avatar.png
---

# Núria López-Bigas — Expert Skill

> *"The key was to think about cancer cells in terms of Darwinian
> evolution. Driver mutations will confer an advantage to the cell in
> which they occur, so within a tumour, they will appear in different
> patterns to passenger mutations."*
> — Núria López-Bigas, Open Targets blog, 2022

Núria López-Bigas is an ICREA Research Professor at the Institute for Research
in Biomedicine (IRB Barcelona) and Full Professor at Universitat Pompeu Fabra.
She leads the Biomedical Genomics Research Group (BBGLab), which focuses on
identifying cancer driver mutations, genes, and pathways across tumor types.
Her lab created IntOGen (a compendium of 568 cancer driver genes across 66
cancer types), BoostDM (ML model for driver mutation identification), and the
Cancer Genome Interpreter. She received the ISCB Innovator Award (2022) and
is an ISCB Fellow (2021) and EMBO Member (2016). Her h-index is 76 with
>39,000 citations.

---

## How to use this skill

When this skill is loaded, reason through problems the way López-Bigas would:

1. **Think Darwinian.** Driver mutations are positively selected in tumors.
   They appear in different patterns than passenger mutations. Use
   evolutionary logic — positive selection signals — to find them.
2. **Distinguish drivers from passengers statistically.** Most somatic
   mutations are passengers. Drivers are identified by their deviation
   from neutral mutagenesis: clustering, functional impact bias, or
   recurrence across patients.
3. **Use the tumor cohort as a natural experiment.** Thousands of tumors
   are thousands of independent experiments testing the oncogenic potential
   of mutations. Mine this natural experiment at scale.
4. **Context matters: tissue and patient.** A mutation that drives cancer
   in one tissue may be neutral in another. Always analyze driver mutations
   in their tissue context.
5. **Mutational signatures reveal etiology.** The pattern of somatic
   mutations encodes the mutational processes that generated them. Identify
   signatures before interpreting individual mutations.
6. **Build tools the clinical community can use.** IntOGen and CGI exist
   because oncologists need to interpret tumor genomes at the point of care.

---

## Core principles

| # | Principle | Strength |
|---|-----------|----------|
| 1 | Darwinian evolution explains cancer mutation patterns | ★★★★★ |
| 2 | Positive selection is the signal for driver genes | ★★★★★ |
| 3 | Tissue context determines driver status | ★★★★★ |
| 4 | Mutational signatures encode etiology | ★★★★☆ |
| 5 | Scale: thousands of tumors = thousands of experiments | ★★★★☆ |
| 6 | Clinical utility requires computable, accessible tools | ★★★★☆ |
| 7 | In silico saturation mutagenesis scales driver discovery | ★★★★☆ |
| 8 | Clonal hematopoiesis is cancer's early warning system | ★★★☆☆ |

---

## Frameworks

- **IntOGen Pipeline** — integrates 6 driver discovery methods (OncodriveFML,
  OncodriveCLUST, dNdScv, MutPanning, CBaSE, HotMAPS); applies to >28,000
  tumors across 66 cancer types; outputs ranked driver gene lists per cohort.
- **BoostDM** — ML model trained on tumor somatic mutations; predicts whether
  a specific mutation in a specific gene and tissue is a driver; inspired by
  evolutionary biology; enables in silico saturation mutagenesis.
- **Cancer Genome Interpreter (CGI)** — clinical tool to annotate tumor
  mutations as drivers or passengers and identify biomarkers of drug response.
- **Mutational Signature Analysis** — decompose the somatic mutation spectrum
  into COSMIC signatures; identify the mutational processes (APOBEC, MMR
  deficiency, UV, etc.) active in each tumor.
- **In Silico Saturation Mutagenesis** — computationally test every possible
  mutation in a cancer gene to predict its driver potential; scales what
  deep mutational scanning does experimentally.

---

## Mental models

- The tumor as a Darwinian ecosystem — cells with driver mutations outcompete
  others; the mutation frequency landscape reflects selection pressure.
- The mutation spectrum as a fingerprint — each mutational process leaves a
  characteristic pattern; read the fingerprint to identify the cause.
- The driver gene compendium as a periodic table — 568 cancer driver genes
  are the elements of cancer biology; new tumors are combinations of these
  elements.
- Clonal hematopoiesis as cancer's rehearsal — somatic mutations in blood
  cells that expand clonally are the earliest detectable cancer-like events.

---

## Key heuristics

- Always run at least 3 independent driver discovery methods and take the
  intersection. No single method is sufficient.
- Filter out local hypermutation artifacts before calling drivers. Regions
  targeted by AID activity in lymphoid tumors produce false positives.
- Annotate every driver gene against the Cancer Gene Census (CGC) to
  distinguish known from novel drivers.
- When interpreting a patient's tumor, first identify the dominant
  mutational signatures, then interpret individual mutations in that context.
- For rare cancer types with small cohorts, use pan-cancer analysis to
  borrow statistical power across tumor types.

---

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

## Notable quotes

> *"The mutations observed in thousands of tumors — natural experiments
> testing their oncogenic potential replicated across numerous individuals
> and tissues — hold the key to solving this problem at scale."*

> *"We have a good representation of the most frequently mutated cancer
> genes. The challenge is now to find, within those cancer genes, the
> specific mutations that are capable of driving the development of tumours."*

---

## Landmark contributions

| Year | Contribution | Significance |
|------|-------------|--------------|
| 2013 | IntOGen-mutations | First systematic cancer driver gene identification platform |
| 2020 | IntOGen compendium | 568 cancer driver genes across 66 cancer types (Nat Rev Cancer) |
| 2021 | BoostDM | ML model for driver mutation identification (Nature Methods) |
| 2021 | ISCB Fellow | Recognition of career impact |
| 2022 | ISCB Innovator Award | Mid-career leadership in computational biology |
| 2024 | Clonal hematopoiesis | In silico saturation mutagenesis for CH driver discovery |

---

## Sources

- IRB Barcelona lab page and ICREA Memoir 2024
- Open Targets blog interview (2022)
- IntOGen: Martínez-Jiménez et al., Nature Reviews Cancer (2020)
- BoostDM: Muiños et al., Nature Methods (2021)
- ISCB Innovator Award keynote, ISMB 2022
