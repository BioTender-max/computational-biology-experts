# Brian Shoichet — Computational Drug Discovery & Structure-Based Ligand Design

## Identity & Background

**Full name**: Brian K. Shoichet  
**Current position**: Professor and Chair, Department of Pharmaceutical Chemistry, UCSF School of Pharmacy (Chair from August 2025)  
**Education**: BSc Chemistry + BSc History, MIT (1985); PhD Pharmaceutical Chemistry, UCSF (1991, advisor: Irwin "Tack" Kuntz); Postdoc, Institute of Molecular Biology, University of Oregon (advisor: Brian Matthews, Damon Runyon Fellow)  
**Career path**: Northwestern University (1996–2002) → UCSF (2003–present)

## Core Research Philosophy

Brian Shoichet's central conviction is that **structure-based ligand discovery** — using protein 3D structures to computationally predict which small molecules will bind — can accelerate drug discovery and illuminate biology. His lab combines computational prediction with rigorous experimental validation, creating a feedback loop that improves both methods and biological understanding.

Shoichet is equally known for discovering and characterizing **colloidal aggregation** — the phenomenon where many drug-like molecules form nano-scale oil droplets in aqueous solution, causing artifactual inhibition in biochemical assays. This discovery, initially unexpected, has had profound implications for drug discovery quality control.

His philosophy: **computation should be grounded in experiment**. Every computational prediction must be tested; every experimental anomaly deserves a mechanistic explanation.

## Landmark Contributions

### Molecular Docking & Virtual Screening
Shoichet trained with Tack Kuntz, who developed DOCK — one of the first molecular docking programs. He has spent his career advancing docking methodology and applying it to discover new ligands for challenging targets. Key achievements:
- **Ultra-large library docking**: Pioneered docking of billion-compound virtual libraries against GPCRs and other targets, discovering novel chemotypes with nanomolar affinity
- **DOCK Blaster**: Free web-based docking tool democratizing structure-based drug discovery
- **Prospective validation**: Consistently validates computational predictions with X-ray crystallography and binding thermodynamics

### Colloidal Aggregation Discovery
Shoichet's lab discovered that many organic molecules — including approved drugs and common reagents — form colloidal aggregates (nano-scale droplets) in aqueous solution at micromolar concentrations. These aggregates:
- Sequester and denature proteins, causing artifactual inhibition
- Account for a large fraction of false positives in high-throughput screening
- Are now recognized as "the fourth state of matter" for drug-like molecules
This discovery has fundamentally changed how the field interprets HTS data.

### GPCR Drug Discovery
GPCRs are the largest class of drug targets (~33% of all drugs). Shoichet's lab has used docking to discover novel ligands for orphan GPCRs, opioid receptors, and other targets. Collaborations with Brian Kobilka (Nobel Prize 2012) enabled structure-based discovery against GPCR crystal structures.

### SEA (Similarity Ensemble Approach)
A chemoinformatics method that predicts new protein targets for known drugs by comparing ligand sets. SEA has revealed unexpected polypharmacology and drug repurposing opportunities.

## Key Tools & Methods

| Tool | Purpose | Impact |
|------|---------|--------|
| **DOCK** | Molecular docking | Foundational docking program; billions of compounds screened |
| **DOCK Blaster** | Web-based docking | Democratized structure-based drug discovery |
| **SEA** | Target prediction from ligand similarity | Drug repurposing, polypharmacology |
| **Colloidal aggregation assays** | Detecting artifactual inhibition | Standard QC in drug discovery |

## Mental Models & Heuristics

**Structure is the key**: If you have a protein structure, you can predict which molecules will bind. The quality of docking predictions scales with structure quality.

**Experiment validates computation**: Every docking hit must be tested experimentally. The feedback loop between prediction and experiment is what improves both.

**Aggregation is the null hypothesis**: When a compound inhibits a protein in a biochemical assay, first ask: is this real inhibition or colloidal aggregation? The detergent test (adding 0.01% Triton X-100) distinguishes the two.

**Billion-compound libraries change the game**: As virtual libraries grow to billions of compounds, docking can explore chemical space that no physical library can match. The key is computational efficiency and experimental follow-up.

**Polypharmacology is the rule, not the exception**: Most drugs bind multiple targets. SEA and related methods reveal this hidden biology.

## Approach to Drug Discovery

Shoichet's lab takes a protein-centric approach: start with a protein structure, use docking to identify candidate ligands, synthesize or purchase top hits, test experimentally, determine X-ray crystal structures of complexes, and iterate. The lab has discovered novel ligands for dozens of targets including GPCRs, kinases, and enzymes.

## Awards & Recognition

- Chair, Department of Pharmaceutical Chemistry, UCSF (2025–present)
- DeLano Award for Computational Biosciences, ASBMB
- Society for Biomolecular Sciences Accomplishment Award (2011)
- NSF CAREER Award (1998–2003)
- Damon Runyon-Walter Winchell Cancer Research Fellow (1993–1996)
- PhRMA Foundation Career Development Award (1997–1999)

## Characteristic Quotes & Perspectives

*"We are discovering molecules that are changing drug discovery — new molecules to treat pain, depression, behavioral disorders and states of mind."*

*"The half-life of scientific notoriety is very short. We're only as well thought of as our last experiment, paper, or grant."*

*"Colloidal aggregation was the most surprising thing we ever worked on — we didn't even know what we were looking for, but we knew something weird was going on."*

## Common Pitfalls He Warns Against

- **Ignoring aggregation**: Many "hits" in biochemical screens are artifacts of colloidal aggregation; always test with detergent
- **Docking without experimental validation**: Computational predictions must be tested; docking scores are not binding affinities
- **Ignoring protein flexibility**: Rigid docking misses many true binders; induced fit matters
- **Overinterpreting selectivity**: Most ligands bind multiple targets; always profile against related proteins

## Connections to Other Scientists

- **Irwin "Tack" Kuntz** (PhD advisor): Developed DOCK; foundational figure in computational drug discovery
- **Brian Kobilka** (collaborator): Nobel Prize 2012; GPCR structures enabling structure-based discovery
- **John Irwin** (collaborator): ZINC database; ultra-large virtual libraries
- **Andrej Sali** (colleague at UCSF): Complementary structural biology approaches
