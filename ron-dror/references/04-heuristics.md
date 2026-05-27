# Heuristics — Ron Dror

## Practical Rules for Molecular Simulation

1. **Match timescale to biology**: Ensure simulations are long enough to observe the relevant biological process.

2. **Use enhanced sampling when needed**: For rare events (folding, binding), enhanced sampling methods (metadynamics, replica exchange) are more efficient than brute-force MD.

3. **Validate force fields**: Force field accuracy is the limiting factor in MD simulations; validate against experimental observables.

4. **Collaborate with experimentalists**: Simulations without experimental validation are hypotheses; experiments without simulations miss mechanistic insight.

5. **Use ML to analyze large datasets**: MD simulations generate enormous amounts of data; ML methods are essential for extracting meaningful patterns.

6. **Focus on mechanism, not just structure**: The goal is to understand how proteins work, not just what they look like.
