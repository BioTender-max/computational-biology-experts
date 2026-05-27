# Core Principles — Anshul Kundaje

## 1. Sequence is Sufficient
Given enough training data, DNA sequence alone contains enough information to predict regulatory activity. The challenge is building models that can learn this mapping.

## 2. Interpretability is Not Optional
A deep learning model that predicts but cannot explain is a black box. TF-MoDISco and similar tools are essential for extracting biological insight from neural networks.

## 3. Base-Pair Resolution Matters
Regulatory logic is encoded at the level of individual base pairs. Models that operate at peak resolution miss the fine-grained combinatorial logic of TF binding.

## 4. Consortia Data Enables Generalization
Models trained on ENCODE and Roadmap data generalize across cell types and species because they have seen the full diversity of regulatory contexts.

## 5. Genetic Variants are the Ultimate Test
A model of gene regulation is only useful if it can predict the effects of genetic variants. Variant effect prediction is the key application of regulatory genomics models.
