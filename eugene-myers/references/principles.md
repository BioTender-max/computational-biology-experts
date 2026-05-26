# Eugene Myers — Core Principles

Frequency-ranked from Caltech Heritage Project interview, ACGT 101 Questions, MPG portrait, ISCB Senior Scientist Award, and published talks.

---

## Principle 1 — Tools Enable Discovery (★★★★★)

**Frequency:** Stated in every major interview and profile.

Myers's foundational belief: the most important contribution a computational scientist can make is not to make discoveries, but to build the tools that make discoveries possible for others. BLAST, the shotgun assembler, the string graph — each was a tool that unlocked a generation of biological research.

> "Having the best tools is really what the game is all about."

> "I produce the tools that allow molecular biologists to discover the things that they discover."

**Implication:** Evaluate your work not by the discoveries you make, but by the discoveries you enable. A tool used by 2 million researchers is more impactful than a discovery made by one lab.

---

## Principle 2 — Algorithm First, Biology Second (★★★★★)

**Frequency:** Caltech Heritage interview, ISCB award, MPG portrait.

Myers came to biology as a mathematician who recognized that DNA sequences were "interesting string problems." He did not start from biological questions and ask what computation was needed — he started from algorithmic problems and found that biology provided the most interesting instances.

> "I just took algorithm design and applied it to computational biology and became an expert in that domain, and in the problems in that domain."

> "Molecular biology was always the place you went, when you didn't want to be quantitative. It didn't involve differential equations and complex things. It was mostly descriptive in the early days."

**Implication:** Bring rigorous algorithmic thinking to biology. The field is full of problems that are, at their core, combinatorial optimization, string matching, or graph theory problems — and most biologists don't know how to solve them.

---

## Principle 3 — Theory Precedes Heuristic (★★★★★)

**Frequency:** Caltech Heritage interview.

BLAST was not invented as a practical tool — it was derived from a theoretical result Myers was already working on. The heuristic came from the theory, not the other way around. This is why BLAST is both fast and principled: it approximates an optimal solution, not an ad hoc one.

> "I was actually trying to do theory. That's what led to BLAST, the search engine. BLAST was basically just a heuristic version of a theoretical result that I was producing, around 1990."

**Implication:** Before building a heuristic, understand the theoretical optimum. A heuristic derived from theory is more robust, more principled, and more likely to generalize than one built by trial and error.

---

## Principle 4 — Solve the Real Problem, Not the Simulated One (★★★★★)

**Frequency:** Caltech Heritage interview, MPG portrait.

Myers's assembly algorithms didn't gain real traction until he went to Celera and had to deal with actual sequencing machines, actual data artifacts, and actual time pressure. "I had to deal with all of the caveats." Proximity to the real problem is essential for building tools that actually work.

> "When I went to Celera, I had to solve a real problem. There was a real factory, real machines, and I had to deal with all of the caveats. That I think was a point at which I began to really be devoted to molecular biology."

**Implication:** Spend time in the lab, at the sequencer, with the data as it actually comes out of the machine. Algorithms designed for idealized data often fail on real data.

---

## Principle 5 — Build for Scale That Doesn't Exist Yet (★★★★☆)

**Frequency:** Caltech Heritage interview, ACGT 101 questions.

Myers consistently thinks ahead to the scale of data that will exist in 10 years, not the scale that exists today. "Many of the codes that we use, they won't scale to what's coming." This forward-looking design philosophy is why his tools have remained relevant across multiple generations of sequencing technology.

> "What are we going to do when we have 100,000 species of genomes sequenced and we want to compare them all? We don't have the software infrastructure in place to do that."

**Implication:** Design algorithms and software for the data volumes of the next decade, not the current decade. Scalability is not an optimization — it is a design requirement.

---

## Principle 6 — Physics Matters More Than Computation (★★★★☆)

**Frequency:** Caltech Heritage interview.

Myers believes that the future of biology requires physicists more than computer scientists. Understanding cellular processes requires understanding phase transitions, condensation, soft-matter physics — not just sequence analysis. "I think physics is probably more important than computation."

> "Understanding what a cell does is not just a question of biochemistry. It's a question of biochemistry and physics... these are biochemical reactions that are taking place in a physical context."

**Implication:** Computational biologists should invest in physics training. The next generation of biological insights will come from understanding the physical context of molecular processes, not just their sequence.

---

## Principle 7 — Cross-Disciplinary Work Requires Cultural Fluency (★★★★☆)

**Frequency:** Caltech Heritage interview.

Myers attributes his success at disciplinary boundaries partly to his multicultural childhood (Pakistan, India, Indonesia, Hong Kong, Japan). Working across disciplines requires understanding that different fields have different cultures — different standards of evidence, different values, different ways of communicating.

> "People are either naïve about the cultural differences, and the fact that they have to be attuned to the cultural differences in the sciences. We're not talking in sociological terms; we're talking about the culture of different scientific fields. Because they have cultures. They really do."

**Implication:** Before collaborating across disciplines, invest time in understanding the other field's culture. What counts as a result? What counts as rigor? What is the standard of proof?

---

## Principle 8 — Data Is Regenerable; Don't Hoard It (★★★★☆)

**Frequency:** "Shifting Ground for Big Data Researchers" profile.

Myers's pragmatic philosophy: if data is cheap to regenerate, don't store it. "Generate it, analyze it, throw it away. If you don't like it a week later, then do it again." This is a mathematician's approach to data — treat it as a computational resource, not a precious artifact.

> "If keeping the data is more expensive [than regenerating it], repeat the experiment rather than store the data."

**Implication:** Distinguish between data that is expensive to regenerate (clinical samples, rare specimens) and data that is cheap (sequencing runs, microscopy images). Apply different storage strategies accordingly.

---

## Principle 9 — Stay in the Code (★★★★☆)

**Frequency:** MPG portrait, Caltech Heritage interview.

Myers writes code himself, first thing every morning, even as a director. He cannot imagine leading a team from behind a desk. The moment a scientist stops doing the work, they lose the ability to make good decisions about it.

> "I just love writing program codes!"

> "He's too much a man of action, too hands-on. Despite his many tasks, he still does his own programming as often as possible: first thing in the morning with the obligatory cappuccino in hand, and occasionally at night or on a plane."

**Implication:** Maintain hands-on engagement with the technical work, even as you take on leadership responsibilities. The best scientific leaders are those who can still do the work.

---

## Principle 10 — The Right Model Organism Is the One You Can Experiment On (★★★★☆)

**Frequency:** Caltech Heritage interview.

Myers is skeptical of the emphasis on human and mouse models in biomedical research. "Why are you doing that in mice, where it takes a year to breed a mouse? You can do the same thing in a fly and it's five days." The right model organism is the one that allows you to do experiments quickly and cheaply.

> "I think that operating and working and trying to understand how the cell works, in whatever kind of experimental system allows you to do that in a facile way, is what we should be investing our money in."

**Implication:** Choose model organisms based on experimental tractability, not on proximity to humans. The insights from tractable systems often transfer to humans anyway.
