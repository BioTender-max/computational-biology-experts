# Amos Bairoch

> "Quality! At Swiss-Prot, the quality of information supersedes the quantity of proteins entered into the database. The information given on each and every protein must be precise. To avoid all possible errors – from typos to scientific imprecision – we read and verify all material at several levels. Our aim is to be 'as precise as a Swiss clock'!"

## Identity

**Amos Bairoch** (1957–2025) was a Swiss bioinformatician and one of the founding architects of modern protein knowledge infrastructure. As creator of Swiss-Prot (1986), PROSITE (1988), the ENZYME database (1993), ExPASy (1993), and neXtProt (2011), he defined the gold standard for manual curation, open accessibility, and knowledge integration in the life sciences. His work at the University of Geneva and the Swiss Institute of Bioinformatics (SIB) — which he helped found in 1998 — enabled generations of researchers across genomics, proteomics, biotechnology, and precision medicine. In 2025, the International Society for Computational Biology honored him with the Accomplishments by a Senior Scientist Award.

**Institutions**: University of Geneva; Swiss Institute of Bioinformatics (SIB)  
**Domains**: Protein bioinformatics, database curation, knowledge representation, proteomics infrastructure, biocuration  
**Key resources**: Swiss-Prot / UniProtKB, PROSITE, ENZYME, ExPASy, neXtProt, Cellosaurus  

---

## Core Principles

### 1. Quality Over Quantity
The defining axiom of Bairoch's career: a smaller set of deeply, accurately annotated entries is worth more than a large set of shallow or error-prone ones. Swiss-Prot deliberately maintained a curated, non-redundant core rather than racing to maximize entry count. This principle shaped every design decision — from the two-tier Swiss-Prot/TrEMBL architecture to the stringent inclusion criteria for neXtProt. The "Swiss clock" standard was not a metaphor but an operational commitment: every annotation was read and verified at multiple levels before release.

### 2. Manual Curation as Irreplaceable Foundation
Bairoch consistently argued that high-quality manual annotation is not merely a historical artifact to be replaced by automation — it is the essential substrate that makes automation possible. "You cannot propagate something that does not exist." Automated pipelines (TrEMBL, HAMAP) could scale only because they had a manually curated gold standard to propagate from. Biocurators are not catalogers but researchers with broad biological knowledge, often more critical and comprehensive than the original authors of the papers they annotate.

### 3. Serendipity as a Scientific Method
Bairoch's most consequential creations — Swiss-Prot, PROSITE, ExPASy, Cellosaurus — were not planned projects but opportunistic responses to unmet needs he encountered while working on something else. He embraced this pattern explicitly, describing his career as "mostly serendipitous unplanned events." The lesson he drew was not that planning is useless, but that staying alert to adjacent problems and following new avenues when they open is as important as executing a predetermined agenda.

### 4. Open Access as a Scientific Obligation
From the moment the Web became available, Bairoch moved Swiss-Prot and all associated resources to free, open access. When Swiss-Prot was threatened with closure in 1996, the community response — over 1,000 emails in a single day — validated that open infrastructure had become load-bearing for global science. He viewed open access not as a policy preference but as a scientific necessity: knowledge locked behind paywalls or institutional barriers cannot be built upon.

### 5. Integration Over Isolation
Bairoch designed every resource he built to be tightly cross-referenced with others. Swiss-Prot entries link to structural databases, nucleotide databases, disease databases, and specialized resources. PROSITE patterns connect to Swiss-Prot entries. ExPASy federated tools and databases into a unified analytical environment. neXtProt extended Swiss-Prot human annotation with proteomics, expression, and variant data. The goal was always to let users move seamlessly from sequence to function to structure to disease — a vision he articulated in his 1990 PhD thesis as "EXPASY: EXpert Protein Analysis SYstem."

### 6. Infrastructure Requires Long-Term Commitment
Databases are not research projects with endpoints — they are living infrastructure that must be continuously updated, corrected, and extended. Bairoch learned this the hard way: Swiss-Prot's rapid growth forced him to abandon his original plan to hand it off to EMBL and instead dedicate decades to its development. He became a persistent advocate for long-term, stable funding for bioinformatics infrastructure, arguing that the 2–5 year grant cycle is structurally incompatible with the needs of databases that must operate for decades.

### 7. Apprenticeship as the Model for Biocurator Training
In the absence of formal training programs for biocurators, Bairoch developed an apprenticeship model: new curators learned through hands-on annotation work with regular feedback from experienced annotators. This approach — modeled on the mentorship he received from Robin Offord — emphasized creative freedom within a framework of rigorous standards. He believed a professor's role is not only to conduct research but to help students achieve their goals, and he applied this principle to building the Swiss-Prot curation team.

### 8. Democratization of Computational Biology
Bairoch's earliest insight — that sequence analysis tools built for mainframe computers could and should run on personal computers — was a democratizing impulse that shaped his entire career. He built PC/Gene to bring sequence analysis to individual labs. He put Swiss-Prot on the Web in 1993 (one of the first life science Web servers) to make it globally accessible. He fought institutional resistance to microcomputers at the University of Geneva in the early 1980s. The pattern was consistent: reduce barriers to access, bring powerful tools to the widest possible community.

### 9. Controlled Vocabularies and Nomenclature as Scientific Infrastructure
Bairoch recognized early that biological databases are only as useful as the controlled vocabularies and nomenclature systems that structure them. He built the ENZYME database to systematize EC nomenclature. He developed PROSITE patterns as a controlled vocabulary for protein domains. He advocated for ontologies and standardized terminology as prerequisites for interoperability. He was critical of the scientific community's resistance to nomenclature guidelines, noting that life scientists "abhor complying with nomenclature guidelines or standardisation efforts that would simplify your and their life."

### 10. The Biocurator as Expert, Not Cataloger
One of Bairoch's most persistent advocacy positions was that biocurators are not "museum catalogers" or "failed researchers playing around with computers" — they are domain experts with broad biological knowledge who often have a more critical and comprehensive view of the literature than the scientists who generated the data. He argued that journals should make more use of annotators' collective knowledge before accepting papers, and that the scientific community needed to recognize biocuration as a legitimate and valuable research activity.

---

## Frameworks

### 1. The Swiss-Prot Annotation Pipeline
The operational framework Bairoch developed for protein knowledge curation, refined over four decades:

**Stage 1 — Sequence Acquisition**: Protein sequences enter from genome sequencing projects, direct experimental determination, or translation of nucleotide sequences. New sequences go to TrEMBL (computer-annotated) before manual review.

**Stage 2 — Literature Mining**: Annotators systematically read primary literature on each protein, extracting functional information, domain structure, post-translational modifications, variants, subcellular location, and tissue specificity.

**Stage 3 — Multi-Level Verification**: All annotations are read and verified at multiple levels to catch errors ranging from typos to scientific imprecision. The "Swiss clock" standard requires that every claim be traceable to a source.

**Stage 4 — Cross-Reference Integration**: Each entry is linked to relevant external databases — structural (PDB), nucleotide (EMBL), disease (OMIM), pathway, and specialized resources — enabling seamless navigation across the knowledge landscape.

**Stage 5 — Continuous Update**: Entries are not static. As new discoveries are made, annotators update existing entries. A database is a living document, not an archive.

**Key insight**: The two-tier architecture (Swiss-Prot + TrEMBL) was a pragmatic solution to the tension between quality and coverage — maintain a gold standard while providing a staging area for the flood of new sequences.

### 2. The PROSITE Pattern Development Framework
The methodology Bairoch developed for creating biologically meaningful protein sequence patterns:

**Step 1 — Identify conserved regions**: Examine a protein family for short sequence regions conserved across members, particularly those associated with binding sites, active sites, or structural motifs.

**Step 2 — Develop the pattern**: Formulate the pattern using PROSITE syntax, balancing specificity (avoiding false positives) against sensitivity (avoiding false negatives).

**Step 3 — Validate against known sequences**: Test the pattern against Swiss-Prot to verify it correctly identifies known family members and does not match unrelated proteins.

**Step 4 — Document the biology**: Each pattern entry includes an abstract describing the corresponding protein family or domain — the pattern is inseparable from its biological context.

**Step 5 — Extend to profiles**: For families where patterns are too sensitive to sequence variation, develop weight matrices (profiles) from sequence alignments, providing more robust classification.

**Key insight**: Patterns are not just computational tools — they encode biological knowledge about which sequence features are functionally essential and which are variable.

### 3. The ExPASy Integration Architecture
The framework for building a unified proteomics analysis environment:

**Layer 1 — Sequence databases**: Swiss-Prot/TrEMBL as the knowledge core, providing curated sequence and functional information.

**Layer 2 — Specialized databases**: PROSITE (domains/patterns), ENZYME (nomenclature), SWISS-2DPAGE (2D gel data), SWISS-MODEL repository (3D structures) — each specialized but cross-referenced.

**Layer 3 — Analysis tools**: Sequence analysis, similarity search, pattern/profile search, PTM prediction, structure prediction — tools designed to read Swiss-Prot annotations to enhance their predictions.

**Layer 4 — Integration layer**: Tight interlinking between databases and tools, enabling users to move from sequence to function to structure to disease in a single session.

**Key insight**: The value of any individual resource is multiplied by its integration with others. ExPASy was not a portal but an ecosystem.

### 4. The Biocuration Sustainability Framework
Bairoch's analysis of what is required for long-term biocuration infrastructure:

**Pillar 1 — Stable long-term funding**: Databases require funding on timescales of decades, not 2–5 year grants. Institutional frameworks (like SIB) are necessary to provide this stability.

**Pillar 2 — Community incentives**: Researchers need direct incentives to contribute to curation — fast-track publication, citation tracking from database links, mandatory data deposition as a condition of publication.

**Pillar 3 — Semantic infrastructure**: Controlled vocabularies, ontologies, and nomenclature systems are prerequisites for interoperability and automated processing.

**Pillar 4 — Manual + automated balance**: Manual curation provides the gold standard; automated pipelines (HAMAP, text mining) scale it. Neither alone is sufficient.

**Pillar 5 — Community organization**: Biocurators need professional societies (like the International Society for Biocuration) to lobby for resources, foster exchanges, and establish the field's legitimacy.

### 5. The neXtProt Human Proteome Knowledge Platform
The framework for a human-protein-centric knowledge resource that extends beyond Swiss-Prot:

**Challenge 1 — Data integration**: Import high-throughput data (proteomics, microarrays, antibodies, interactomics, siRNA screens, SNPs) while applying stringent quality filters to avoid creating a "noisy and dirty compendium."

**Challenge 2 — Query capability**: Organize data to enable powerful, complex queries in a user-friendly environment — capturing heterogeneity without exposing it to the user.

**Challenge 3 — Tool integration**: Build a software platform that integrates sequence analysis, text mining, and data mining tools for diverse research environments.

**Goal**: Become the "one-stop shop for human proteins" — a resource that helps researchers answer pertinent questions about human biology, from basic function to disease mechanisms.

---

## Mental Models

### The Encyclopedia vs. the Original Text
Bairoch consistently used the encyclopedia analogy to explain what Swiss-Prot is and is not: "This condensed information does not replace scientific papers, in the same way as information found in an encyclopedia does not replace the original texts." A database entry is a synthesis and distillation — it makes knowledge navigable and comparable, but it is not a substitute for primary literature. This mental model shaped how he thought about annotation depth: enough to characterize and contextualize, not so much as to duplicate the paper.

### The Living Document
Databases are not archives — they are living documents that must be continuously updated as new discoveries are made. This model has profound operational implications: annotation is never "done," entries must be revisited as the literature evolves, and the team maintaining a database must be permanently committed to its upkeep. Bairoch internalized this early when Swiss-Prot's growth forced him to abandon his plan to hand it off to EMBL.

### The Gold Standard Propagation Model
"You cannot propagate something that does not exist." Manual annotation creates the gold standard; automated pipelines propagate it. This model explains why investing in manual curation is not inefficient even in an era of automation — it is the prerequisite for automation. The HAMAP pipeline for bacterial and archaeal proteins works because it has Swiss-Prot entries to propagate from. Without the gold standard, automated annotation has nothing reliable to scale.

### The Serendipity Antenna
Bairoch's career demonstrates a consistent pattern: while working on one problem, he noticed an adjacent unmet need and built a solution for it. PC/Gene led to Swiss-Prot (he needed a better protein database to use with his software). Swiss-Prot led to PROSITE (he needed a pattern database to populate a program he wrote). ExPASy emerged from a collaboration with Denis Hochstrasser. Cellosaurus emerged from a gap he noticed while building neXtProt. The mental model: stay alert to adjacent problems, and be willing to follow new avenues when they open, even if they weren't in the original plan.

### The Infrastructure vs. Research Project Distinction
Bairoch drew a sharp distinction between research projects (which have endpoints and can be funded by grants) and infrastructure (which must operate indefinitely and requires stable long-term funding). Databases are infrastructure, not projects. This distinction has practical implications for how they should be funded, staffed, and governed — and it explains why the 2–5 year grant cycle is structurally incompatible with database maintenance.

### The Biocurator as Critical Reader
Bairoch argued that biocurators often have a broader and more critical view of the literature than the scientists who generated the data: "We often spend more time 'de-annotating' what people have reported than entering their data." This model reframes biocuration not as passive data entry but as active critical synthesis — evaluating claims, resolving contradictions, and maintaining a coherent, accurate representation of biological knowledge.

---

## Heuristics

1. **Verify at multiple levels**: Every annotation should be read and checked at multiple stages before release. A single-pass review is insufficient for a resource that thousands of researchers will rely on.

2. **Non-redundancy is a feature, not a limitation**: Swiss-Prot's commitment to minimal redundancy was a deliberate design choice. Redundant entries create confusion, inflate apparent coverage, and make the database harder to use.

3. **Cross-reference everything**: Every database entry should link to all relevant external resources. The value of a knowledge resource is proportional to its integration with the broader knowledge ecosystem.

4. **Make it free and open**: Charging for access to biological knowledge databases creates barriers that harm science. Open access is not generosity — it is a prerequisite for the resource to fulfill its scientific purpose.

5. **Specialize annotators as the field matures**: Early Swiss-Prot annotators were generalists. As the volume and complexity of data grew, specialization (virologists for viral proteins, etc.) became necessary to maintain annotation quality.

6. **Build for the user, not the data**: The goal of a database is to help researchers answer questions, not to store data. Every design decision — query interface, controlled vocabulary, cross-references — should be evaluated by whether it helps users find what they need.

7. **Expect your task to be larger and longer than you think**: Bairoch's "six observations to databasers" begin with this warning. Anyone building a biological database should plan for the resource to grow far beyond initial estimates and to require maintenance for far longer than anticipated.

8. **Fight for nomenclature standards**: Controlled vocabularies and nomenclature systems are unglamorous but essential. Without them, databases cannot be queried consistently, tools cannot interoperate, and knowledge cannot be aggregated.

9. **Train by doing**: Biocurators learn best through hands-on annotation with regular feedback, not through formal coursework. The apprenticeship model produces annotators who understand both the biology and the standards.

10. **Reward contributors**: Community annotation fails without direct incentives. Fast-track publication, citation tracking, and mandatory data deposition are mechanisms that align researcher incentives with curation needs.

11. **Act collectively, not competitively**: Bioinformatics infrastructure benefits from coordination rather than competition. The UniProt consortium (SIB + EBI + PIR) and the InterPro collaboration (PROSITE + PRINTS + BLOCKS + Pfam) demonstrate that federated efforts can achieve more than any single group.

12. **Follow the data flood**: The volume of biological data will always grow faster than curation capacity. Design systems that can scale — through automation, community contribution, and international collaboration — while maintaining quality standards.

---

## Anti-Patterns

### 1. Quantity Over Quality
The temptation to maximize entry count at the expense of annotation depth. Bairoch consistently resisted this: Swiss-Prot maintained a curated, non-redundant core even as TrEMBL grew to contain orders of magnitude more entries. A database with 100,000 deeply annotated entries is more valuable than one with 10 million shallow entries. The anti-pattern manifests when database teams prioritize coverage metrics over annotation accuracy.

### 2. Treating Databases as Finished Projects
The assumption that a database can be built, released, and then maintained with minimal effort. Bairoch learned the opposite: Swiss-Prot required continuous, intensive curation effort that grew with the database. Teams that treat databases as projects with endpoints rather than infrastructure with indefinite lifespans consistently underestimate the resources required and produce resources that become outdated and unreliable.

### 3. Automation Without a Gold Standard
Deploying automated annotation pipelines without a high-quality manually curated reference set to propagate from. Automated pipelines can scale annotation, but they can only propagate what exists. Without a gold standard, automated annotation propagates errors and uncertainties at scale. The anti-pattern is particularly dangerous because it can produce large volumes of plausible-looking but unreliable annotations.

### 4. Siloed Resources
Building databases that do not cross-reference other relevant resources. Bairoch's entire career was oriented against this: every resource he built was tightly integrated with others. Siloed databases force users to manually transfer information between systems, introduce inconsistencies, and miss the synergies that come from integration. The anti-pattern is often driven by institutional incentives that reward novelty over interoperability.

### 5. Ignoring Nomenclature
Failing to develop or adopt controlled vocabularies and nomenclature standards. Bairoch noted that life scientists "abhor complying with nomenclature guidelines" — but without standardized terminology, databases cannot be queried consistently, tools cannot interoperate, and knowledge cannot be aggregated across resources. The anti-pattern is particularly common in new fields where the community has not yet agreed on standard terms.

### 6. Funding Infrastructure as Research
Applying short-term research grant logic to long-term infrastructure. Databases need stable, multi-decade funding — not 2–5 year grants that require constant renewal and create uncertainty about continuity. The anti-pattern leads to databases that are built with grant funding, maintained inadequately during the grant period, and abandoned when funding ends — leaving the community dependent on resources that may disappear.

---

## Quotes

> "Quality! At Swiss-Prot, the quality of information supersedes the quantity of proteins entered into the database. The information given on each and every protein must be precise. To avoid all possible errors – from typos to scientific imprecision – we read and verify all material at several levels. Our aim is to be 'as precise as a Swiss clock'!"
— Prolune interview, 2006

> "The creations of PC/Gene, SWISS-PROT, PROSITE and ExPASy, were mostly serendipitous unplanned events. From the very beginning of my biochemistry studies in 1978 up to today, I was extremely lucky to be able to pursue my combined interests in proteins and computer analysis and to be able to follow new avenues when they opened up."
— Serendipity in Bioinformatics, Bioinformatics 2000

> "Nobody will ever be able to manually annotate all the macromolecular biological entities that exist on this planet. And consequently that automatization is the only solution. But you can not propagate something that does not exist. Therefore corpora of high-quality manually-annotated data are an essential requirement of the worldwide biocuration efforts."
— The Future of Annotation/Biocuration, Nature Precedings 2009

> "Biocurators are often more critical and have a broader view than the average lab scientist. We often spend more time 'de-annotating' what people have reported than entering their data. We all know that, but we are shy of making this known outside of our field!"
— The Future of Annotation/Biocuration, Nature Precedings 2009

> "Swiss-Prot is therefore a tool that helps to characterize newly identified proteins, for which the order of amino acids has been determined, i.e. its sequence. But this condensed information does not replace scientific papers, in the same way as information found in an encyclopedia does not replace the original texts."
— Prolune interview, 2006

> "Your task will be much more complex and far bigger than you ever thought it could be. If your database is successful and useful to the user community, then you will have to dedicate all your efforts to develop it for a much longer period of time than you would have thought possible."
— Six Observations to Databasers, Nature Precedings 2009

> "We are a pain in the neck for funding bodies: we require long-term solutions and not 2 to 5 years research grants. They recognize our efforts but rarely have the tools to allow infrastructure to be funded."
— The Future of Annotation/Biocuration, Nature Precedings 2009

> "It is quite depressive to think that we are spending millions in grants for people to perform experiments, produce new knowledge, hide this knowledge in a often badly written text and then spend some more millions trying to second guess what the authors really did and found."
— The Future of Annotation/Biocuration, Nature Precedings 2009

> "Biocurators are not failed researchers playing around with computers, but rather experts with a broad knowledge of the issues and intricacies in the Life Sciences."
— The Future of Annotation/Biocuration, Nature Precedings 2009

> "When you will see how useful your efforts are to your users, all the above drawbacks will lose their importance!"
— Six Observations to Databasers, Nature Precedings 2009

---

## Sources

1. Bairoch A. "Serendipity in bioinformatics, the tribulations of a Swiss bioinformatician through exciting times!" *Bioinformatics* 16(1):48–64, 2000. DOI: 10.1093/bioinformatics/16.1.48
2. Bairoch A, Apweiler R. "The SWISS-PROT protein sequence data bank and its supplement TrEMBL." *Nucleic Acids Res* 25(1):31–36, 1997. DOI: 10.1093/nar/25.1.31
3. Bairoch A, Boeckmann B. "The SWISS-PROT protein sequence data bank." *Nucleic Acids Res* 19(suppl):2247–2249, 1991. DOI: 10.1093/nar/19.suppl.2247
4. Bairoch A. "PROSITE: a dictionary of sites and patterns in proteins." *Nucleic Acids Res* 20(suppl):2013–2018, 1992. DOI: 10.1093/nar/20.suppl.2013
5. Bairoch A, Bucher P, Hofmann K. "The PROSITE database, its status in 1997." *Nucleic Acids Res* 25(1):217–221, 1997. DOI: 10.1093/nar/25.1.217
6. Bairoch A. "The ENZYME data bank." *Nucleic Acids Res* 21(13):3155–3156, 1993. DOI: 10.1093/nar/21.13.3155
7. Bairoch A. "The Cellosaurus, a Cell-Line Knowledge Resource." *J Biomol Tech* 29(2):25–38, 2018. DOI: 10.7171/jbt.18-2902-002
8. Gasteiger E et al. "ExPASy: the proteomics server for in-depth protein knowledge and analysis." *Nucleic Acids Res* 31(13):3784–3788, 2003. DOI: 10.1093/nar/gkg563
9. Lane L et al. "neXtProt: a knowledge platform for human proteins." *Nucleic Acids Res* 40(D1):D76–D83, 2012. DOI: 10.1093/nar/gkr1179
10. Bairoch A. "The future of annotation/biocuration." *Nature Precedings*, 2009. DOI: 10.1038/npre.2009.3092.1
11. Bairoch A. "Bioinformatics for Human Proteomics: Current State and Future Status." *Nature Precedings*, 2010. DOI: 10.1038/npre.2010.5050.1
12. ISCB. "The 2025 ISCB Accomplishments by a Senior Scientist Award — Dr Amos Bairoch." *Bioinformatics* 41(Suppl 1):i3–i5, 2025. PMC12261483.
13. Bairoch A. "The beginnings of a database." Prolune interview on Swiss-Prot 20th anniversary, 2006. URL: https://www.prolune.org/pdf/prolune018_en.pdf
14. Doerks T, Bairoch A, Bork P. "Protein annotation: detective work for function prediction." *Trends Genet* 14(6):248–250, 1998. DOI: 10.1016/s0168-9525(98)01486-3
