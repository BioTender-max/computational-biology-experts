# David Baker — Mental Models

How Baker thinks about proteins, science, AI, and time.

---

## 1. Protein folding as biological self-organization

Baker came to think of protein folding as "the simplest case of biological
self-organization." This framing — proteins as the minimal unit of
self-organization — is what drew him from cell biology to structural biology
and ultimately to protein design.

**Why it matters:** If you understand the simplest case of self-organization,
you gain leverage on all more complex cases (cells, tissues, organisms). Protein
folding is the entry point to understanding how order emerges from sequence.

**Implication for design:** If folding is self-organization, then design is
*directed* self-organization — specifying the sequence so that the system
self-organizes into the structure you want.

> *"I sort of came to think of it as the simplest case of biological
> self-organization."*
> — C&EN profile, 2019

---

## 2. The energy landscape

Protein folding and design are fundamentally about navigating an energy
landscape. The native structure is the global energy minimum. Misfolded
structures are local minima. Design means constructing a sequence whose energy
landscape has a deep, narrow minimum at the desired structure — and no
competing minima that could trap the protein in a wrong shape.

**Practical implication:** When a designed protein doesn't fold correctly, the
energy landscape has the wrong shape — either the desired minimum isn't deep
enough, or there are competing minima. The fix is to redesign the sequence to
steepen the funnel toward the target structure.

**Historical note:** Rosetta was built on this physical intuition — Monte Carlo
sampling of conformational space to find the lowest-energy structure. Deep
learning methods (RFdiffusion, ProteinMPNN) learned the same landscape
implicitly from data.

---

## 3. AI as pattern recognition, not understanding

Baker is clear-eyed about what AI does: it recognizes patterns in large
datasets. AlphaFold succeeded because 50+ years of structural biology produced
a massive, curated dataset. The rules of protein folding are still "opaque" —
AI found the patterns without revealing the principles.

**The key distinction:**
- Pattern recognition: given enough examples, predict the output for new inputs
- Understanding: know *why* the output is what it is, from first principles

**Where this matters:** AI works spectacularly when there is a large, curated
dataset and a well-posed prediction task. It struggles when:
- The dataset is small or noisy
- The task is open-ended (design, not prediction)
- You need to extrapolate far beyond the training distribution

**The over-extrapolation warning:** Don't assume that because AI solved protein
structure prediction, it will solve all of biology. As you move up the
biological complexity hierarchy (proteins → cells → tissues → organisms), the
datasets get smaller and the tasks get more open-ended.

> *"The rules [of protein folding] are still opaque, but it was pattern
> recognition that solved the problem."*
> — Nobel Prize podcast, 2024

> *"I think the extrapolation from what's been done with protein structure
> prediction and protein design, people may be over-extrapolating."*
> — Existential Hope podcast

---

## 4. The 3-month horizon

Baker plans 3 months ahead and has "a little bit of an inkling beyond there."
This is not a limitation — it is a deliberate choice. A 3-month horizon:

- Keeps you responsive to new information
- Prevents over-commitment to a path that may become wrong
- Keeps you in the adjacent possible rather than chasing distant fantasies
- Forces you to re-evaluate priorities regularly

**The paradox:** Baker's 3-month horizon has produced 30+ years of
groundbreaking science. Long-term vision is not the same as long-term planning.
You can have a grand vision (design proteins to solve humanity's problems) while
planning only 3 months ahead.

> *"I like to try and see 3 months out, and that gives me some intuition about
> what problems are good and what directions will be profitable."*
> — C&EN profile, 2019

---

## 5. Proteins as molecular machines

Every biological function — neural signaling, muscle movement, immune response,
photosynthesis — is mediated by a specific protein. Proteins are atomically
reproducible, nanoscale machines. This framing (proteins as machines, not just
molecules) is what makes protein design feel like engineering rather than
chemistry.

**Why the framing matters:**
- "Molecule" suggests chemistry: reactions, concentrations, equilibria
- "Machine" suggests engineering: function, design, specification, iteration

**The engineering implication:** If proteins are machines, then protein design
is machine design. You specify the function you want, design the machine to
perform it, build it, test it, and iterate. This is exactly how Baker's lab
operates.

**The nanotechnology connection:** Baker explicitly connects protein design to
Eric Drexler's vision of molecular machines. The difference: Baker is actually
building them, using biology's own machinery (ribosomes, DNA synthesis) as the
fabrication platform.

---

## 6. Data as fossil fuel

The protein structure database (PDB) is like fossil fuel: 50+ years and tens
of billions of dollars of global scientific effort, accumulated slowly and then
burned rapidly by AI. This is why AI worked so spectacularly for protein
structure prediction.

**The implication:** As you move up the biological complexity hierarchy, you
don't have equivalent datasets. Cell biology, developmental biology, and
whole-organism behavior lack the PDB's scale, curation, and precision. AI's
power diminishes accordingly.

**The warning:** Don't assume that because AI burned the protein-structure
fossil fuel so effectively, it will find equivalent fuel elsewhere in biology.
The fuel has to be there first.

> *"It's kind of like the fossil fuel; we burned fast because there was all
> this stuff that was done before."*
> — Existential Hope podcast
