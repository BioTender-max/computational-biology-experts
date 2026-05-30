# Mental Models — Amos Bairoch

## 1. The Encyclopedia vs. the Original Text

Bairoch consistently used the encyclopedia analogy to explain what Swiss-Prot is and is not: "This condensed information does not replace scientific papers, in the same way as information found in an encyclopedia does not replace the original texts."

**What this means operationally**: A database entry is a synthesis and distillation — it makes knowledge navigable and comparable, but it is not a substitute for primary literature. The annotator's job is to extract, synthesize, and contextualize, not to reproduce the paper. This mental model shaped how Bairoch thought about annotation depth: enough to characterize and contextualize, not so much as to duplicate the paper.

**The implication for users**: A Swiss-Prot entry tells you what is known about a protein — its function, domains, modifications, variants — and points you to the papers where that knowledge was established. It is a map, not the territory.

**Why it matters**: This model prevents two failure modes: (1) annotations that are too shallow to be useful, and (2) annotations that try to reproduce the full complexity of the primary literature and become unmanageable. The encyclopedia standard defines the right level of abstraction.

---

## 2. The Living Document

Databases are not archives — they are living documents that must be continuously updated as new discoveries are made. This model has profound operational implications: annotation is never "done," entries must be revisited as the literature evolves, and the team maintaining a database must be permanently committed to its upkeep.

**The operational consequence**: "A database is not static: as new discoveries are made, the information must follow." Annotators do not just add new entries — they continuously update existing ones. A protein annotated in 1990 may need to be substantially revised in 2000 and again in 2010 as new experimental evidence accumulates.

**The staffing consequence**: Because annotation is never done, the team maintaining a database must be permanently engaged with the literature. This is why Swiss-Prot grew from one person (Bairoch in 1986) to over 70 staff by 2006 — not because the database grew larger, but because the literature grew faster.

**The funding consequence**: Living documents require living budgets. The 2–5 year grant cycle is structurally incompatible with a resource that must be maintained indefinitely. This is why Bairoch fought for institutional solutions (SIB) rather than relying on grant funding.

---

## 3. The Gold Standard Propagation Model

"You cannot propagate something that does not exist." Manual annotation creates the gold standard; automated pipelines propagate it. This model explains why investing in manual curation is not inefficient even in an era of automation — it is the prerequisite for automation.

**The logic**: Automated annotation pipelines work by propagating known annotations to new sequences based on similarity. If the known annotations are wrong, the propagated annotations will be wrong at scale. If the known annotations are shallow, the propagated annotations will be shallow at scale. The quality of the gold standard determines the quality of everything built on top of it.

**The HAMAP example**: The HAMAP pipeline for bacterial and archaeal proteins works because it has Swiss-Prot entries to propagate from. It is "probably one of the most reliable automatic annotation pipelines operationally deployed" — because it propagates from a high-quality manual reference.

**The implication for AI**: As machine learning models are trained on biological databases, the quality of the training data determines the quality of the models. A model trained on Swiss-Prot will be more reliable than one trained on TrEMBL, because Swiss-Prot's annotations are more accurate and consistent.

---

## 4. The Serendipity Antenna

Bairoch's career demonstrates a consistent pattern: while working on one problem, he noticed an adjacent unmet need and built a solution for it. The mental model is not that serendipity is random — it is that staying alert to adjacent problems and being willing to follow new avenues when they open is a learnable and cultivatable skill.

**The pattern**:
- Working on PC/Gene → noticed NBRF/PIR was poorly formatted → built Swiss-Prot
- Building Swiss-Prot → wrote a pattern-scanning program → needed patterns → built PROSITE
- Working on ExPASy → collaborated with Denis Hochstrasser → built SWISS-2DPAGE and SWISS-MODEL
- Building neXtProt → noticed no central cell line database existed → built Cellosaurus

**The prerequisite**: Serendipity requires intellectual freedom and institutional support. Bairoch was able to follow these new avenues because Offord gave him freedom to pursue his interests, and because the resources he built generated enough value to justify continued investment.

**The lesson for researchers**: The most important discoveries often come from noticing what is missing, not from executing a predetermined plan. Maintaining awareness of adjacent problems — and having the flexibility to pursue them — is a core scientific skill.

---

## 5. The Infrastructure vs. Research Project Distinction

Bairoch drew a sharp distinction between research projects (which have endpoints and can be funded by grants) and infrastructure (which must operate indefinitely and requires stable long-term funding). Databases are infrastructure, not projects.

**The practical implications**:
- Research projects can be funded by 2–5 year grants; infrastructure cannot
- Research projects have defined endpoints; infrastructure does not
- Research projects can be staffed by postdocs and students; infrastructure requires permanent staff
- Research projects produce papers; infrastructure produces resources that enable other research

**The funding mismatch**: "We are a pain in the neck for funding bodies: we require long-term solutions and not 2 to 5 years research grants. They recognize our efforts but rarely have the tools to allow infrastructure to be funded." The Swiss national fund supported research projects, not infrastructure — which is why Swiss-Prot nearly closed in 1996.

**The institutional solution**: The Swiss Institute of Bioinformatics was created specifically to provide the institutional framework for long-term bioinformatics infrastructure funding. It operates under Article 16 of the Swiss Federal Constitution, which authorizes the Confederation to finance non-profit research of national interest.

---

## 6. The Biocurator as Critical Reader

Bairoch argued that biocurators often have a broader and more critical view of the literature than the scientists who generated the data: "We often spend more time 'de-annotating' what people have reported than entering their data."

**What this means**: Biocuration is not passive data entry — it is active critical synthesis. Annotators evaluate claims, resolve contradictions between papers, identify errors and overinterpretations, and maintain a coherent, accurate representation of biological knowledge. They read papers more carefully and more broadly than most researchers, because they must integrate information across hundreds of papers on a single protein.

**The "de-annotation" phenomenon**: When a paper reports a finding that contradicts established knowledge, or that turns out to be an artifact, biocurators must remove or qualify the annotation. This is invisible work — it does not generate papers or citations — but it is essential for maintaining the accuracy of the knowledge base.

**The implication for peer review**: "Journals should make more use of the collective knowledge of annotators before accepting a paper for publication." Biocurators, who have read the entire literature on a protein family, are often better positioned to evaluate a new paper's claims than the typical peer reviewer.
