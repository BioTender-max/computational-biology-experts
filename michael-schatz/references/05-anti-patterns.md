# Michael Schatz — Anti-Patterns

## Anti-Pattern 1 — Using short reads for structural variant detection
Short reads cannot span most structural variants. Using short reads for SV detection will miss the majority of SVs. Use long reads instead.

## Anti-Pattern 2 — Ignoring structural variants
Most genomics studies focus on SNPs and small indels. But structural variants are often more functionally important. Don't ignore structural variants.

## Anti-Pattern 3 — Using a single assembler
Different assemblers have different strengths and weaknesses. Always compare multiple assemblers and choose the best for your data.

## Anti-Pattern 4 — Ignoring ploidy
Polyploid genomes require specialized assembly tools. Using a diploid assembler for a polyploid genome will produce incorrect results.

## Anti-Pattern 5 — Not using cloud computing for large-scale genomics
Local clusters are insufficient for large-scale genomics. Use cloud computing to scale to the appropriate data volume.

## Anti-Pattern 6 — Ignoring diversity
Most human genomics studies have been conducted in populations of European ancestry. This limits the generalizability of findings. Include diverse populations in genomics studies.

## Anti-Pattern 7 — Not validating SVs with orthogonal methods
Structural variants detected by a single method may be false positives. Always validate SVs with orthogonal methods (long reads, short reads, optical mapping).
