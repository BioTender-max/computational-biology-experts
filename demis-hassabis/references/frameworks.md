# Demis Hassabis — Frameworks

Five structured frameworks extracted from Nobel lecture, interviews, and public talks.

---

## Framework 1 — The Search-Model-Objective (SMO) Framework

**Source:** Nobel lecture "Accelerating Scientific Discovery with AI" (Dec 2024)

The core insight behind AlphaFold, AlphaGo, and Hassabis's broader AI philosophy: most hard problems are tractable once reframed as a search problem with three components.

**Three conditions for AI tractability:**
1. **Massive combinatorial search space** — the problem must be too large for brute force
2. **Clear objective function** — there must be a metric to optimize against
3. **Data or simulator** — either lots of training data, or an accurate environment to learn from

**The general solution:**
1. Learn a model of the environment (from data or simulation)
2. Use that model to guide search according to the objective function
3. Iterate: model improves search, search improves model

**Applications:**
- Protein folding: search space = 10^300 conformations; objective = minimum free energy; data = PDB
- Drug discovery: search space = chemical space; objective = binding affinity + selectivity; data = assays
- Go: search space = 10^170 positions; objective = win; simulator = the game itself

**Key quote:** "Taking a step back, what is the essence of what our systems are doing? Finding the optimal solution in an enormous combinatorial space. Learn a model of that environment. Use that model to guide a search according to an objective function. Turns out this is a very general solution and many problems fit this approach."

---

## Framework 2 — Digital Biology

**Source:** Nobel lecture, Die Zeit interview, CBS 60 Minutes

A paradigm shift: biology is not a wet science constrained by experimental throughput — it is an information science that can be accelerated by orders of magnitude using AI.

**The analogy:**
- Physics → Mathematics (elegant equations: F=ma, E=mc²)
- Biology → AI (emergent, interactive, multi-signal systems)

**Three pillars of Digital Biology:**
1. **Structural biology at scale** — AlphaFold predicts all 200M+ known protein structures
2. **Drug discovery at digital speed** — Isomorphic Labs compresses years of drug design into months
3. **Virtual cell** — a computational model of a cell that can be perturbed in silico

**Key quote:** "AlphaFold is a proof point that could usher in a new era of 'digital biology'... We sometimes think of this as doing Science at Digital Speed."

**Implication:** The bottleneck in biology is no longer data collection — it is computational interpretation. AI transforms biology from an experimental science into a computational one.

---

## Framework 3 — Games as Proving Ground

**Source:** Nobel interview, Nobel lecture, multiple career retrospectives

Hassabis used games systematically as a three-stage ladder for AI development:

**Stage 1 — Personal cognitive training (chess, age 4–17)**
Games train pattern recognition, strategic planning, and the ability to evaluate positions under uncertainty. Chess "was very formative with the way that I think about the world and formative of how I approach problems."

**Stage 2 — AI development laboratory (game design, age 17–26)**
Writing AI for commercial games (Theme Park, Black & White) was Hassabis's first laboratory for exploring AI algorithms in real environments with real constraints.

**Stage 3 — AI proving ground (DeepMind, 2010–present)**
Games provide the ideal conditions for testing learning algorithms: clear rules, measurable outcomes, no ambiguity about success. AlphaGo → AlphaZero → AlphaFold is a direct lineage.

**The three conditions games satisfy:**
- Massive combinatorial space (Go: 10^170 positions)
- Clear objective (win/lose)
- Accurate simulator (the game itself)

**Key quote:** "Games have been a critical part of my entire career... using games as a test bed, a proving ground for the AI systems to learn."

---

## Framework 4 — The Interdisciplinary Polymath Model

**Source:** Nobel interview, TIME100, Sequoia interview

Hassabis's model for building world-class research teams and for his own intellectual development.

**Individual level:**
- Develop genuine depth in at least two fields (not just surface familiarity)
- Seek the "in-between points" where fields connect
- Be willing to be a generalist in a world that rewards specialists

**Team level:**
- Assemble people with world-class depth in different domains
- Create a "melting pot" where different epistemic cultures collide
- Ensure no single person could do the work alone

**DeepMind's original team composition:**
- Machine learning engineers
- Neuroscientists
- Mathematicians
- Later: philosophers, ethicists, chemists, physicists

**Key quote:** "In DeepMind, in our research groups, we've always had at the beginning, multidisciplinary groups... A lot of the strength of the work we do comes from that, including things like AlphaFold, which is a big collaboration between people with very different world class skills in their own areas."

---

## Framework 5 — Responsible AGI Development

**Source:** Nobel lecture, Die Zeit, Nobel interview, CBS 60 Minutes

Hassabis's framework for navigating the dual-use risks of increasingly powerful AI systems.

**Two primary risk categories:**
1. **Bad actors** — general-purpose AI repurposed for harmful ends by individuals or rogue states
2. **Technical AGI risk** — systems that become self-improving and develop unintended goals

**Response framework:**
1. **Proactive stakeholder engagement** — consult biosecurity, bioethics, government, academia before release
2. **International coordination** — safety is only meaningful if it's global; unilateral safety is insufficient
3. **Transparency about uncertainty** — acknowledge what we don't know about these systems
4. **Structural safety research** — mechanistic interpretability, alignment, monitoring tools

**The threshold:** Hassabis's personal red line is "advanced, generalized agents that could operate through world models" — systems that are active in the world, not just passive responders.

**Key quote:** "Technology as transformative as AGI requires exceptional care and foresight... Critical to engage with a wide range of stakeholders from government, academia, and civil society."
