# Mental Models — David Haussler

Reasoning patterns, metaphors, and lenses Haussler applies to problems.

---

## 1. The Exponential Leverage Lens

**Description**: When a method scales linearly with data and data grows
exponentially, the scientific output grows exponentially. This is not just
a computational fact — it is a scientific strategy.

**Example**: HMMs scale linearly with sequence data. DNA sequencing improved
10× every two years (hyper-Moore's Law). The combination produced exponential
scientific leverage: from thousands of bases in the 1980s to 3 billion bases
in 2000 to millions of genomes today.

**Application**: Before choosing a method, ask: what is its scaling law? What
is the growth law of the data? If the method scales worse than the data grows,
it will become a bottleneck.

**Source**: PLOS Genetics interview (2013)

---

## 2. The Conservation Filter

**Description**: Before investing experimental resources in a genomic region,
ask: is it conserved across species? Conservation is a free, high-signal filter.

**Example**: HAR1 was identified by scanning for regions that were highly
conserved across amniotes but showed accelerated change in humans. This
computational filter identified a candidate that turned out to be expressed
in the developing human cortex — a result that would have been nearly
impossible to find by experiment alone.

**Application**: Use phastCons/phyloP scores as a first filter before any
experimental investment. Regions conserved for 500 million years are almost
certainly functional. Regions that are not conserved are probably not worth
the experiment.

**Source**: Pollard et al. (2006) Nature; iBiology talk (2014)

---

## 3. The Reference Bias Trap

**Description**: Any analysis anchored to a single linear reference genome is
systematically biased against individuals whose genomes differ from that reference.

**Example**: GRCh38 was built from a small number of individuals, mostly of
European ancestry. Structural variants, insertions, and population-specific
sequences are invisible. Studies using GRCh38 as ground truth systematically
undercount variation in non-European populations.

**Application**: Always ask: whose genomes are represented in this reference?
What variation is invisible? Use the pangenome when possible. Report reference
bias as a limitation.

**Source**: Human Pangenome Reference Consortium (2023) Nature

---

## 4. The Unified Framework Advantage

**Description**: When you see five different tools solving the same problem with
different formalisms, the right move is to find the unifying mathematical framework.

**Example**: Before HMMs, gene finding used weight matrices, protein homology
used BLAST, and RNA structure used thermodynamic models. HMMs unified all three
under one probabilistic framework, enabling principled extensions (phylo-HMMs,
discriminative HMMs) that none of the ad hoc tools could support.

**Application**: When you encounter a proliferation of tools for the same problem,
look for the shared mathematical structure. The unified framework will scale better,
extend more naturally, and reveal the underlying biology more clearly.

**Source**: PLOS Genetics interview (2013); Siepel & Haussler (2003, 2005)

---

## 5. The Open Internet as Scientific Infrastructure

**Description**: The decision to post the human genome on the internet in 2000
was not just ethical — it was the correct scientific strategy. Open access
accelerates the entire field faster than any single lab's proprietary advantage.

**Example**: Celera's subscription model was immediately outcompeted by the
freely posted UCSC genome. The UCSC Genome Browser became the standard tool
for the field precisely because it was open. Infrastructure that enables sharing
is as valuable as the data itself.

**Application**: Default to open. Design for federation. Use standard APIs.
Post everything on the internet. The network effects of open data always dominate.

**Source**: PLOS Genetics interview (2013); UCSC Genome Browser history

---

## 6. The Evolutionary Telescope

**Description**: The genome is a record of billions of years of evolutionary
experiments. Comparative genomics is a telescope that lets you read that record.

**Example**: By comparing human, chimpanzee, mouse, dog, and chicken genomes,
Haussler's team could identify which of the 15 million changes since the
human-chimp ancestor were under positive selection. This is impossible from
a single genome.

**Application**: Before running any experiment, look through the evolutionary
telescope. Every conserved element is a hypothesis about function; every
accelerated region is a hypothesis about innovation. The telescope is free —
use it first.

**Source**: iBiology talk (2014); Haussler (2008) ACM STOC "Computing how we
became human"

---

## 7. Conway's Game of Life as a Model of Emergence

**Description**: Simple mathematical rules can generate arbitrarily complex
self-replicating patterns. Life itself may be an emergent property of
sufficiently complex information-processing systems.

**Example**: Haussler uses Conway's Game of Life as a mental model for thinking
about the origin of life: "you start with a random pattern, and you will have
emergent forms that will be self-replicating entities that interact, as in
living systems."

**Application**: When thinking about biological complexity, ask: what are the
simple rules that generate this complexity? Is this an emergent property of
a simpler underlying system?

**Source**: PLOS Genetics interview (2013)
