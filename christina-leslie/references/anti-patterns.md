# Christina Leslie — Anti-Patterns

Failure modes that Leslie's work explicitly or implicitly argues against.

## 1. Algorithm-first thinking
Designing a clever algorithm before asking what biological question it answers. Mathematicians are attached to elegant solutions; biologists need meaningful insights. The algorithm is secondary to the question.

## 2. Single-gene studies
Studying one gene at a time when genome-wide data is available. The power of next-generation sequencing is that it enables global, unbiased measurement of biological processes. Use it.

## 3. Generative models for prediction
Using overrepresentation-based motif discovery when discriminative models are more powerful for prediction. The goal is to learn what distinguishes functional from non-functional sequences, not to describe what is overrepresented.

## 4. Ignoring 3D genome structure
Modeling gene regulation from 1D epigenomic data alone. Distal enhancers regulate gene expression through 3D chromatin interactions; models that ignore 3D structure miss key regulatory logic.

## 5. Computational isolation
Working without close collaboration with experimental labs. Computational predictions must be validated experimentally. Close collaboration with wet-lab scientists is essential for both validation and problem formulation.

## 6. Modest ambition
Tackling only tractable problems rather than the most important ones in cancer. MSKCC's culture encourages ambitious science; computational scientists should match that ambition.

## 7. Unvalidated predictions
Publishing computational predictions without experimental validation. CRISPRi, TAP-seq, and other functional assays are essential for validating regulatory predictions.
