# Trey Ideker — Mental Models

## The Network Module Principle
Biological networks are organized into modules (protein complexes, pathways). Mutations cluster within modules. Understanding modular organization is the key to understanding how perturbations propagate.

## The Guilt-by-Association Heuristic
Genes that interact with known disease genes are more likely to be disease genes themselves. Network proximity is a universal predictor of biological relationships.

## The Synthetic Lethality Opportunity
Cancer cells have one gene of a synthetic lethal pair already inactivated. Targeting the partner gene selectively kills cancer cells while sparing normal cells.

## The Hierarchy of Biological Organization
Atoms → molecules → complexes → pathways → processes → cells → tissues → organisms. VNNs exploit this hierarchy by constraining model architecture to mirror it.

## The Perturbation-Response Matrix
The fundamental data structure of systems biology: rows = perturbations, columns = responses. The pattern of responses reveals network structure. Genes with similar response profiles are functionally related.

## The Visible vs. Black Box Distinction
A VNN that achieves 90% accuracy and tells you why is more valuable than a black box that achieves 95% accuracy and tells you nothing. Interpretability is not a luxury in medicine.
