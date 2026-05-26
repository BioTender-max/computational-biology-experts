# Demis Hassabis — Heuristics

20 actionable heuristics across 5 categories, distilled from Nobel interview, lecture, Die Zeit, TIME100, CBS, Big Technology Podcast.

---

## Category A — Problem Selection

**H1. The Three-Condition Test**
Before committing to an AI project, verify: (1) Is the search space massive? (2) Is there a clear objective function? (3) Is there data or a simulator? If any condition is missing, build it first.

**H2. Pick Problems at Field Intersections**
The highest-value problems live where two fields meet but haven't yet been connected. Actively map the boundaries of your fields and look for unconnected nodes.

**H3. Monitor Enabling Conditions, Not Just Ideas**
Maintain a list of your most ambitious problems alongside their enabling conditions (data, compute, methods, talent). When conditions ripen, move immediately.

**H4. Prefer Grand Challenges with Clear Benchmarks**
CASP was the benchmark that made protein folding tractable as a research problem. Seek problems with gold-standard benchmarks — they provide unambiguous feedback and motivate the community.

---

## Category B — Research Execution

**H5. Embed Domain Knowledge as Inductive Biases**
Don't treat AI as a generic function approximator. Encode what you know about the domain (physics, evolution, geometry) directly into the architecture. This is not "cheating" — it is good science.

**H6. Use Iterative Refinement**
AlphaFold2's "recycling" stage iteratively refines predictions. Build feedback loops into your systems: initial prediction → refinement → better prediction. Iteration is often more powerful than a single forward pass.

**H7. Validate Against Atomic-Level Ground Truth**
AlphaFold's threshold was <1.0Å average error — the width of an atom. Set your validation criteria at the level of precision that actually matters to practitioners, not at the level that's easy to achieve.

**H8. Build End-to-End Systems**
Avoid pipelines where each stage is optimized independently. End-to-end training allows the system to discover representations that serve the final objective, not intermediate proxies.

---

## Category C — Team and Organization

**H9. Hire for Depth in Complementary Domains**
Don't hire generalists who are mediocre at everything. Hire world-class specialists in different domains and create the conditions for them to collaborate. The intersection is where the magic happens.

**H10. Maintain a Melting Pot Culture**
Actively mix ML engineers, domain scientists, mathematicians, and ethicists. Resist the tendency for disciplines to self-segregate. Physical proximity and shared problems accelerate cross-pollination.

**H11. Stay Involved in the Work**
Hassabis remained technically engaged with AlphaFold throughout its development. Leaders who lose touch with the technical details lose the ability to make good architectural decisions.

---

## Category D — Open Science and Impact

**H12. Open-Source Your Core Tools**
If your tool could enable work you cannot do yourself, release it. The compounding returns from the global scientific community vastly exceed what any single lab can achieve. Open science is the highest-leverage strategy.

**H13. Measure Impact by Downstream Use**
The true measure of AlphaFold's impact is not citations — it is the 2M+ researchers who used it for applications DeepMind never imagined. Design for downstream use, not just for publication.

**H14. Collaborate with Nonprofits and Global Health**
Hassabis specifically partnered with DNDi (Drugs for Neglected Diseases) to apply AlphaFold to diseases that big pharma ignores. Seek collaborations where your tools have disproportionate impact on underserved problems.

---

## Category E — Career and Mindset

**H15. Treat Each Success as a Launchpad, Not a Destination**
Hassabis acknowledges he is "not that good at celebrating successes" because each one immediately motivates the next, bigger ambition. Use success as fuel, not as a resting point.

**H16. Believe in Your Ideas Before Others Do**
"Perhaps I had less faith in that than I should have had. That those ideas would bear fruit, with enough passion and work and effort." Confidence in your ideas from an early stage is critical — not arrogance, but conviction.

**H17. Design Your Career Around Your Passions**
"I don't really think of things as work-life balance... I've designed my work to sort of be my life passions." The most productive researchers are those for whom work and life are indistinguishable.

**H18. Learn from Diverse Cultures and Contexts**
Hassabis's interdisciplinary approach was shaped partly by his multicultural upbringing and his chess training. Seek experiences that force you to see problems from radically different perspectives.

**H19. Engage Publicly on Societal Implications**
Scientists working on transformative technologies have an obligation to engage with policymakers, the public, and civil society. This is not a distraction from research — it is part of the responsibility.

**H20. Maintain Humility About What You Don't Know**
"We don't understand anything about the nature of reality really. We have some approximations, but they have holes in them." The deepest questions remain open. Stay curious about what you don't know.
