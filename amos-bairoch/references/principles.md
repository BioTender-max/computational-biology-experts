# Principles — Amos Bairoch

## 1. Quality Over Quantity

The defining axiom of Bairoch's career: a smaller set of deeply, accurately annotated entries is worth more than a large set of shallow or error-prone ones. Swiss-Prot deliberately maintained a curated, non-redundant core rather than racing to maximize entry count. This principle shaped every design decision — from the two-tier Swiss-Prot/TrEMBL architecture to the stringent inclusion criteria for neXtProt.

**Operational expression**: "Quality! At Swiss-Prot, the quality of information supersedes the quantity of proteins entered into the database. The information given on each and every protein must be precise. To avoid all possible errors – from typos to scientific imprecision – we read and verify all material at several levels. Our aim is to be 'as precise as a Swiss clock'!" (Prolune interview, 2006)

**Structural consequence**: The two-tier architecture (Swiss-Prot + TrEMBL) was a pragmatic solution to the tension between quality and coverage. TrEMBL provided a staging area for the flood of new sequences; Swiss-Prot maintained the gold standard. The 250,000 manually annotated Swiss-Prot entries required a cumulative total of 600 person-years over 23 years — approximately 420 entries per year per FTE.

**Evidence**: Bairoch & Apweiler, *Nucleic Acids Res* 1997; Bairoch, *Nature Precedings* 2009.

---

## 2. Manual Curation as Irreplaceable Foundation

Bairoch consistently argued that high-quality manual annotation is not merely a historical artifact to be replaced by automation — it is the essential substrate that makes automation possible. "You cannot propagate something that does not exist." Automated pipelines (TrEMBL, HAMAP) could scale only because they had a manually curated gold standard to propagate from.

**The biocurator's role**: Biocurators are not catalogers but researchers with broad biological knowledge, often more critical and comprehensive than the original authors of the papers they annotate. "Biocurators are often more critical and have a broader view than the average lab scientist. We often spend more time 'de-annotating' what people have reported than entering their data."

**Scale of the challenge**: Annotating all 4,957 proteins of *Schizosaccharomyces pombe* required approximately 10 person-years — reading ~1,600 pombe-specific papers and carefully propagating information from other eukaryotic organisms.

**Evidence**: Bairoch, *Nature Precedings* 2009; ISCB Award profile, *Bioinformatics* 2025.

---

## 3. Serendipity as a Scientific Method

Bairoch's most consequential creations — Swiss-Prot, PROSITE, ExPASy, Cellosaurus — were not planned projects but opportunistic responses to unmet needs he encountered while working on something else. He embraced this pattern explicitly, describing his career as "mostly serendipitous unplanned events."

**The pattern**:
- PC/Gene → Swiss-Prot: while developing sequence analysis software, he needed a better protein database and built one
- Swiss-Prot → PROSITE: while building Swiss-Prot, he wrote a pattern-scanning program and needed patterns to populate it
- ExPASy: emerged from a collaboration with Denis Hochstrasser on proteomics tools
- Cellosaurus: noticed a gap in cell line resources while building neXtProt

**The lesson**: Staying alert to adjacent problems and following new avenues when they open is as important as executing a predetermined agenda. The serendipity was not accidental — it required the intellectual flexibility to recognize an unmet need and the institutional freedom to pursue it.

**Evidence**: Bairoch, *Bioinformatics* 2000; ISCB Award profile, *Bioinformatics* 2025.

---

## 4. Open Access as a Scientific Obligation

From the moment the Web became available, Bairoch moved Swiss-Prot and all associated resources to free, open access. When Swiss-Prot was threatened with closure in 1996, the community response — over 1,000 emails in a single day — validated that open infrastructure had become load-bearing for global science.

**Historical context**: Swiss-Prot began as a resource distributed on magnetic tapes for a delivery charge. With the advent of the Internet and then the Web, it became "totally free of charge so that those interested worldwide could benefit." ExPASy launched on 1 August 1993 — one of the first life science Web servers, when fewer than 150 Web servers existed worldwide.

**The 1996 crisis**: When European funding fell through and Swiss-Prot faced closure, Bairoch sent an appeal on ExPASy. The same day, over 1,000 emails and letters of support arrived, triggering coverage in Nature and Science and pressure on the Swiss Federal Parliament. The crisis ultimately led to the creation of the Swiss Institute of Bioinformatics.

**Evidence**: Bairoch, *Bioinformatics* 2000; Prolune interview, 2006.

---

## 5. Integration Over Isolation

Bairoch designed every resource he built to be tightly cross-referenced with others. Swiss-Prot entries link to structural databases, nucleotide databases, disease databases, and specialized resources. PROSITE patterns connect to Swiss-Prot entries. ExPASy federated tools and databases into a unified analytical environment. neXtProt extended Swiss-Prot human annotation with proteomics, expression, and variant data.

**The vision**: In his 1990 PhD thesis conclusions, Bairoch wrote: "Ideally one would like to present a protein sequence to a protein analysis system and obtain from this system some hints regarding the function of that protein, its similarities to other known proteins, if possible a tertiary structure model, and finally propositions for experiments that would prove or disprove some of the conclusions obtained by the system." He called this system "EXPASY: for EXpert Protein Analysis SYstem."

**Practical expression**: Swiss-Prot entries cross-reference ~100 external databases. ExPASy tools are designed to read Swiss-Prot annotations to enhance their predictions. InterPro unified PROSITE, PRINTS, BLOCKS, PRODOM, and Pfam into a single protein family/domain identification system.

**Evidence**: Bairoch, *Bioinformatics* 2000; Gasteiger et al., *Nucleic Acids Res* 2003.

---

## 6. Infrastructure Requires Long-Term Commitment

Databases are not research projects with endpoints — they are living infrastructure that must be continuously updated, corrected, and extended. Bairoch learned this the hard way: Swiss-Prot's rapid growth forced him to abandon his original plan to hand it off to EMBL and instead dedicate decades to its development.

**The funding problem**: "We are a pain in the neck for funding bodies: we require long-term solutions and not 2 to 5 years research grants. They recognize our efforts but rarely have the tools to allow infrastructure to be funded." The Swiss national fund supported research projects, not infrastructure. European funds were refused. The 1996 crisis forced the creation of SIB as an institutional solution.

**The physicist model**: Bairoch argued that bioinformaticians should learn from physicists, who secured long-term funding for large-scale infrastructure (CERN, synchrotrons) by acting collectively and embedding themselves in decision-making processes for research budget allocation.

**Evidence**: Bairoch, *Nature Precedings* 2009; Prolune interview, 2006.

---

## 7. Apprenticeship as the Model for Biocurator Training

In the absence of formal training programs for biocurators, Bairoch developed an apprenticeship model: new curators learned through hands-on annotation work with regular feedback from experienced annotators. This approach was modeled on the mentorship he received from Robin Offord.

**Offord's influence**: Offord sheltered Bairoch from faculty criticism of his computational PhD project, fought for the purchase of the first Apple II microcomputer in Switzerland for Bairoch's use, and gave him the freedom to commercialize PC/Gene and use the royalties to hire staff. The greatest lesson: "a professor's role is not only to conduct research, but to help students achieve their goals."

**Application to biocuration**: As Swiss-Prot expanded, Bairoch's most significant mentoring impact was through training biocurators — granting young researchers maximum creative freedom while encouraging senior scientists to step back and empower the next generation.

**Evidence**: ISCB Award profile, *Bioinformatics* 2025; Prolune interview, 2006.

---

## 8. Democratization of Computational Biology

Bairoch's earliest insight — that sequence analysis tools built for mainframe computers could and should run on personal computers — was a democratizing impulse that shaped his entire career. He built PC/Gene to bring sequence analysis to individual labs. He put Swiss-Prot on the Web in 1993 to make it globally accessible. He fought institutional resistance to microcomputers at the University of Geneva in the early 1980s.

**The microcomputer battle**: From 1982 to 1984, Bairoch and Offord fought against computer scientists who believed microcomputers were "fit only for computer games such as 'space invaders'" and would never be useful for science. The victory — obtaining the first Apple II microcomputer in Switzerland for Bairoch — was a turning point.

**The Web as democratizer**: ExPASy was accessed 7,295 times in its first month (August 1993). A few years later, it was accessed at a rate of more than 2 million times per month, from 151 countries.

**Evidence**: Bairoch, *Bioinformatics* 2000; Prolune interview, 2006; ISCB Award profile, *Bioinformatics* 2025.

---

## 9. Controlled Vocabularies and Nomenclature as Scientific Infrastructure

Bairoch recognized early that biological databases are only as useful as the controlled vocabularies and nomenclature systems that structure them. He built the ENZYME database to systematize EC nomenclature. He developed PROSITE patterns as a controlled vocabulary for protein domains. He advocated for ontologies and standardized terminology as prerequisites for interoperability.

**The nomenclature problem**: "You will always wonder why life scientists abhor complying with nomenclature guidelines or standardisation efforts that would simplify your and their life." Despite this resistance, Bairoch consistently pushed for standardization, arguing that without controlled vocabularies, databases cannot be queried consistently and tools cannot interoperate.

**The ENZYME database**: Created to provide a repository of information related to enzyme nomenclature, based on the recommendations of the Nomenclature Committee of the International Union of Biochemistry and Molecular Biology (IUBMB). It became an indispensable resource for the development of metabolic databases.

**Evidence**: Bairoch, *Nucleic Acids Res* 1993 (ENZYME); Bairoch, *Nature Precedings* 2009.

---

## 10. The Biocurator as Expert, Not Cataloger

One of Bairoch's most persistent advocacy positions was that biocurators are not "museum catalogers" or "failed researchers playing around with computers" — they are domain experts with broad biological knowledge who often have a more critical and comprehensive view of the literature than the scientists who generated the data.

**The museum curator analogy**: "I believe this is a misleading analogy: biocurators are much more curators than catalogers. Museum curators were/are researchers that have made tremendous contributions to the natural sciences. As long as we are seen as catalogers, the value of what we provide is not going to be judged by its intrinsic value."

**Practical implication**: Journals should make more use of annotators' collective knowledge before accepting papers. The scientific community needs to recognize biocuration as a legitimate and valuable research activity, not a second-tier support function.

**Evidence**: Bairoch, *Nature Precedings* 2009; ISCB Award profile, *Bioinformatics* 2025.
