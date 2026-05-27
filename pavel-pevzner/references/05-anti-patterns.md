# Pavel Pevzner — Anti-Patterns

## Anti-Pattern 1 — Using the wrong graph formulation
Using an overlap graph (Hamiltonian path) instead of a de Bruijn graph (Eulerian path) for short-read assembly leads to NP-hard problems. Always use the correct mathematical formulation.

## Anti-Pattern 2 — Ignoring repeats
Genome assembly without a principled approach to repeat resolution produces fragmented, incorrect assemblies. Always consider the repeat structure of the genome.

## Anti-Pattern 3 — Skipping error correction
Assembling error-prone reads without error correction produces spurious branches in the de Bruijn graph. Always error-correct reads before assembly.

## Anti-Pattern 4 — Using a single assembler
Different assemblers have different strengths and weaknesses. Always compare multiple assemblers and choose the best for your data.

## Anti-Pattern 5 — Not validating the assembly
An assembly without quality assessment is not a contribution. Always use QUAST, BUSCO, and other tools to assess assembly quality.

## Anti-Pattern 6 — Treating bioinformatics as just "applying computers to biology"
This view diminishes the intellectual content of bioinformatics. The de Bruijn graph and breakpoint graph are mathematical contributions, not just engineering tools.

## Anti-Pattern 7 — Ignoring the sequencing technology
The optimal assembly algorithm depends on the sequencing technology. Don't use a short-read assembler for long reads.
