# Fabian Theis — Core Principles

## 1. Cell State as a Continuous Manifold
Cells exist on a continuous manifold of states, not in discrete categories. Single-cell RNA-seq samples points on this manifold. The goal is to learn the geometry of this manifold.

## 2. RNA Velocity: Time from Splicing Kinetics
The ratio of unspliced to spliced mRNA encodes the direction of transcriptional change. RNA velocity transforms static snapshots into dynamic trajectories.

## 3. Optimal Transport for Cell Fate Mapping
Single-cell experiments are destructive — you cannot track the same cell over time. Optimal transport provides a principled framework for inferring trajectories from static snapshots.

## 4. Open Source as a Scientific Philosophy
Science advances faster when tools are shared freely. The scverse ecosystem (scanpy, AnnData, scVI, CellRank, moscot) is the foundation of modern single-cell analysis because it is open, documented, and community-maintained.

## 5. Foundation Models for Cell Biology
Large pre-trained models trained on massive single-cell datasets can learn universal representations of cell biology. These representations can be fine-tuned for specific tasks.

## 6. Batch Effects are the Enemy of Discovery
Technical variation (batch effects) must be removed while preserving biological signal. scVI's approach: condition the decoder on batch as a known covariate.

## 7. Reference Atlases as Coordinate Systems
Cell atlases provide reference coordinate systems for cell biology. New datasets can be mapped onto these references using transfer learning (scArches).
