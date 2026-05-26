# Bernhard Schölkopf — Conceptual Frameworks

## Framework 1: Kernel Methods and the Kernel Trick
**Problem**: Many real-world problems are non-linear, but linear methods are tractable and well-understood.

**Solution**: Map data into a high-dimensional feature space (reproducing kernel Hilbert space, RKHS) where linear methods apply. The kernel function k(x, x') computes inner products in this space without explicitly computing the mapping φ(x).

**Key insight**: The kernel trick makes it possible to work in infinite-dimensional feature spaces efficiently. The SVM only needs pairwise kernel evaluations, not explicit feature vectors.

**Applications**: SVMs for classification, kernel PCA for dimensionality reduction, kernel-based independence tests (HSIC) for causal discovery, Gaussian processes.

---

## Framework 2: Structural Causal Models (SCMs)
**Problem**: Statistical models describe correlations but cannot answer interventional or counterfactual questions.

**Solution**: Structural causal models — systems of equations X_i = f_i(PA_i, N_i) where PA_i are the causal parents of X_i and N_i are independent noise variables.

**Three levels of causal reasoning** (Pearl's ladder):
1. **Association**: P(Y | X) — what is correlated with what?
2. **Intervention**: P(Y | do(X=x)) — what happens if we intervene?
3. **Counterfactual**: P(Y_x | X=x', Y=y') — what would have happened?

**Key insight**: SCMs can answer all three levels. Statistical models can only answer level 1.

---

## Framework 3: Independent Causal Mechanisms (ICM) Principle
**Principle**: The causal mechanisms that generate data are independent of each other. The mechanism P(X_i | PA_i) is independent of the mechanism P(PA_i).

**Implications**:
- **Causal discovery**: The direction of causation can be identified from observational data using asymmetries in the joint distribution
- **Transfer learning**: Mechanisms that are stable across environments can be identified and transferred
- **Semi-supervised learning**: The marginal distribution P(X) contains information about the causal direction

**Additive noise models**: X → Y if Y = f(X) + N_Y, where N_Y ⊥ X. The direction of causation can be identified from the residuals.

---

## Framework 4: Causal Representation Learning
**Problem**: The key open problem in AI: learning high-level causal variables from low-level observations (pixels, sequences, sensor readings).

**Goal**: Learn representations that correspond to the causal variables of the world — variables that are stable across interventions and distribution shifts.

**Approach**:
1. Identify independent causal mechanisms in the data
2. Learn representations that disentangle these mechanisms
3. Validate by testing stability under distribution shift

**Connection to biology**: In genomics, the causal variables are genes, proteins, and pathways — not raw sequence data. Learning these representations from data is the fundamental challenge.
