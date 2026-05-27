# Rahul Satija — Mental Models

## The Integration Imperative
Single datasets are limited by their experimental context. Integration across datasets reveals conserved biology that is invisible in any single dataset.

## The Modality Weight Intuition
Different cells have different information content in different modalities. A T cell is better defined by protein markers; a stem cell by RNA. WNN learns this automatically.

## The Sketch as a Representative Sample
A sketch is a representative subset of cells that captures the full diversity of the dataset. Analysis on the sketch generalizes to the full dataset via dictionary learning.

## The Reference Atlas as a Coordinate System
A cell atlas provides a reference coordinate system. New datasets are mapped onto this coordinate system, enabling automated annotation and cross-dataset comparison.

## The Batch Effect as a Nuisance Variable
Batch effects are technical variation that must be removed while preserving biological signal. CCA anchors identify cells that represent the same biological state in different batches.
