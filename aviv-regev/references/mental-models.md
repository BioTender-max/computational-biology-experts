# Aviv Regev — Mental Models

Six core mental models that shape how Regev perceives problems and makes decisions.

---

## Mental Model 1 — Smoothie vs. Fruit Salad

**Source:** MIT Technology Review, EMBO profile

Regev's most famous analogy: bulk RNA sequencing is like a smoothie — once you blend millions of cells together, you can't distinguish the individual fruits. Single-cell RNA sequencing is like a fruit salad — you can see each blueberry, raspberry, and blackberry separately.

**The model:**
- Bulk measurement = smoothie (average of all cells)
- Single-cell measurement = fruit salad (individual cell profiles)
- The smoothie hides the heterogeneity that drives biology
- The fruit salad reveals it

**Application:** Before designing any genomics experiment, ask: am I making a smoothie or a fruit salad? If the question involves cell type heterogeneity, rare cell types, or cell state transitions, you need a fruit salad.

**Key quote:** "Previous techniques required blending many different cells together to have enough material to study, making it challenging to distinguish a particular type of cell, more like trying to pick out the blueberries from a smoothie made from many other types of fruit."

---

## Mental Model 2 — The Miro Pixel Sampling Principle

**Source:** EMBO profile

Regev uses a visual demonstration in her talks: a blank slide fills pixel by pixel with dashes of yellow and red. Long before the picture is complete, viewers can make out Joan Miro's "Painting, March 13, 1933." The structure is recognizable from a sample — you don't need every pixel.

**The model:**
- You don't need to sequence all 37 trillion cells to understand the Human Cell Atlas
- A representative sample reveals the structure
- More cells at lower depth often beats fewer cells at higher depth
- The key is sampling breadth, not measurement depth

**Application:** When designing large-scale profiling experiments, optimize for sampling breadth. The goal is to cover the space of cell types, not to exhaustively characterize each cell.

---

## Mental Model 3 — The Circuit Wiring Diagram

**Source:** MIT Technology Review

Regev thinks of gene regulatory networks as circuits — wiring diagrams that describe how molecular signals flow through the cell. Understanding the cell requires understanding the circuit topology, not just the list of components.

**The model:**
- Proteins on the cell surface = input nodes
- Signaling networks = wires and logic gates
- Transcription factors = amplifiers and switches
- Gene expression programs = outputs

**Application:** When analyzing gene expression data, don't just ask "what genes are expressed?" Ask "what is the circuit topology?" How do signals flow from input to output? Where are the bottlenecks? Where are the feedback loops?

**Key quote:** "The protein signaling networks are like 'circuits' — and you can think about the cell 'almost like a wiring diagram.'"

---

## Mental Model 4 — Disease as Cellular Deviation

**Source:** AACR 2024, MIT Tech Review, BioCentury

Regev's model of disease: disease is not a property of a tissue or an organ — it is a property of specific cells in specific states. Understanding disease requires identifying which cells have deviated from their healthy state and how.

**The model:**
- Healthy tissue = reference cell states
- Disease = deviation from reference states
- Drug target = the mechanism driving the deviation
- Drug = intervention that corrects the deviation without affecting healthy states

**Application:** When studying a disease, first build the healthy reference. Then identify the cells that have deviated. Then find the gene programs that define the deviation. Then target those programs.

**Example — Melanoma:**
Regev found that some melanoma cells were resistant to therapy from the start — not because they acquired resistance, but because they were in a pre-existing resistant state. This reframed the question from "how do cells acquire resistance?" to "what is the resistant cell state?"

---

## Mental Model 5 — The Vector Field of Team Leadership

**Source:** "Design for inference" podcast

Regev's model for leading large scientific teams: instead of directing individuals, create a "vector field" — a shared direction that allows team members to move independently while all pointing toward the same goal.

**The model:**
- A vector field assigns a direction to every point in space
- Each team member is a point in the space of possible research directions
- The leader's job is to define the field, not to direct each individual
- When the field is well-defined, individuals can make autonomous decisions that are collectively coherent

**Application:** When leading a large team or consortium, invest in defining the shared vision and the shared standards. Then trust team members to make autonomous decisions within that framework.

---

## Mental Model 6 — The Periodic Table Prediction Principle

**Source:** MIT Technology Review, Human Cell Atlas white paper

Just as the periodic table made it possible to predict the existence of elements that hadn't yet been observed, the Human Cell Atlas will make it possible to predict the existence of cell types that haven't yet been found.

**The model:**
- The periodic table organized elements by properties → revealed gaps → predicted undiscovered elements
- The Human Cell Atlas organizes cells by molecular identity → will reveal gaps → will predict undiscovered cell types

**Application:** When building a reference map, look for gaps. Where are the missing cell types? What cell types should exist based on the structure of the atlas but haven't been found yet? These gaps are research opportunities.

**Key quote:** "Just as the periodic table made it possible to predict the existence of elements yet to be observed, the Human Cell Atlas could help us predict the existence of cells that haven't been found."
