# Frameworks — Andrej Sali

## Integrative Modeling Platform (IMP)
A formal framework for integrative/hybrid structure determination:
1. **Representation**: Define the model representation (atoms, beads, domains)
2. **Restraints**: Encode all experimental data as spatial restraints
3. **Sampling**: Sample the space of possible structures (Monte Carlo, MD)
4. **Analysis**: Identify structures consistent with all restraints
5. **Validation**: Validate against independent data
6. **Deposition**: Deposit in PDB-Dev

## MODELLER Workflow
1. Identify homologous template structures (BLAST, HHpred)
2. Align target sequence to template(s)
3. Generate restraints from alignment and template structure
4. Optimize model by satisfying restraints
5. Assess model quality (DOPE score, QMEAN)
6. Refine and validate

## Spatiotemporal Modeling
Extending integrative modeling to capture dynamics:
- Model structures at multiple time points
- Integrate time-resolved data (FRET, HDX-MS)
- Build spatiotemporal models of cellular processes
