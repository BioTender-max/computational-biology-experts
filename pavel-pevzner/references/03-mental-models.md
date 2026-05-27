# Pavel Pevzner — Mental Models

## "Genome assembly as an Eulerian path problem"
The key insight: assembly = finding an Eulerian path through a de Bruijn graph. This transforms an NP-hard problem into a linear-time problem. The right mathematical formulation changes everything.

## "Repeats as the enemy of assembly"
Genome assembly is hard because of repeats. Every assembly algorithm must have a principled approach to repeat resolution. Long reads help by spanning repeats.

## "The graph as a model of the genome"
The de Bruijn graph, repeat graph, and breakpoint graph are all models of the genome — they capture different aspects of genome structure. The right graph model reveals the right algorithm.

## "Bioinformatics as combinatorial mathematics"
Genome assembly, sequence alignment, and phylogenetics are all combinatorial mathematics problems. The right mathematical formulation reveals the correct algorithm.

## "Education as force multiplication"
A textbook or Coursera course that teaches 100,000 students the right way to think about bioinformatics has more impact than any individual research paper.

## "Long reads as a new paradigm"
Short reads require de Bruijn graph assembly; long reads enable repeat graph assembly. The transition is a qualitative change in the assembly problem, not just a quantitative one.
