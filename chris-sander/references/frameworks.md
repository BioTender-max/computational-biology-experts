# Frameworks — Chris Sander

---

## 1. The Co-Evolution Contact Prediction Pipeline

**When to apply**: Predicting residue-residue contacts and 3D structure from
multiple sequence alignments, without experimental structure data.

**Steps**:
1. Collect a large, diverse multiple sequence alignment (hundreds to thousands
   of sequences) for the protein family
2. Compute pairwise correlated mutations between all residue positions
3. Apply maximum entropy / direct coupling analysis (DCA) to disentangle direct
   from indirect (transitive) correlations
4. Rank residue pairs by direct coupling strength
5. Use top-ranked pairs as distance constraints for 3D structure calculation
6. Validate against known structures; iterate on the statistical model

**Source**: Göbel, Sander et al. (1994) Proteins; Marks, Sander et al. (2011)
PLoS ONE (EVfold)

---

## 2. The Perturbation Biology Modeling Framework

**When to apply**: Building predictive models of cancer cell responses to drugs
and drug combinations.

**Steps**:
1. Select a cancer cell line or patient-derived organoid
2. Apply systematic perturbations: single drugs, drug pairs, gene knockdowns
3. Measure rich molecular readouts (proteomics, phosphoproteomics, transcriptomics)
   at multiple time points
4. Use machine learning (CellBox, Bayesian networks) to infer a network model
   from perturbation-response data
5. Validate the model by predicting responses to held-out perturbations
6. Use the validated model to predict effective drug combinations that block
   resistance escape pathways

**Source**: Yuan, Sander et al. (2021) Cell Systems; Bio-IT World keynote (2015)

---

## 3. The DSSP Secondary Structure Assignment Protocol

**When to apply**: Assigning secondary structure to any protein with known 3D
coordinates; creating a standard for comparison across studies.

**Steps**:
1. Read atomic coordinates from PDB/mmCIF format
2. Calculate optimal hydrogen bond positions (1.000 Å from backbone N)
3. Compute H-bond energies between all atom pairs
4. Identify the best two H-bonds for each atom
5. Assign secondary structure based on repeating H-bond patterns:
   - Repeating turns → helices (α, 3₁₀, π)
   - Repeating bridges → ladders → sheets (β)
   - Bends, loops, coils for remaining residues
6. Report solvent exposure and geometric features

**Source**: Kabsch & Sander (1983) Biopolymers 22:2577–2637

---

## 4. The Cancer Combination Therapy Design Workflow

**When to apply**: Identifying drug combinations that prevent resistance in
targeted cancer therapy.

**Steps**:
1. Profile the cancer's molecular landscape (genomics, proteomics, signaling)
2. Identify the "main essence" — the 3–5 key pathways driving survival and growth
3. Build a perturbation biology model of the cancer cell's signaling network
4. Simulate single-drug responses; identify resistance escape pathways
5. Predict drug combinations that simultaneously block the primary target and
   all identified escape routes
6. Validate predictions in preclinical models (cell lines, organoids, PDX)
7. Design basket or match clinical trials based on shared genomic alterations

**Source**: Bio-IT World keynote (2015); Dana-Farber/MSKCC lab description

---

## 5. The Sequence-Structure Fitness Framework

**When to apply**: Detecting remote homologs or predicting fold class when
sequence identity is below 25% (the twilight zone).

**Steps**:
1. Build a contact profile for the query protein from its 3D structure
2. Derive sequence preferences for each contact interface type from the database
3. Generate hypothetical models by threading the query sequence through all
   known structures in all possible alignments
4. Score each model by summing sequence preferences over all structural positions
5. Incorporate evolutionary information (core weights from multiple alignments)
6. Select the model with the best sequence-structure fitness score

**Source**: Ouzounis, Sander et al. (1993) JMB 232:805–825
