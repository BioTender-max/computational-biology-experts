# Heuristics — Brian Shoichet

## Practical Rules for Computational Drug Discovery

1. **Always test for aggregation**: Before concluding that a compound is a true inhibitor, rule out colloidal aggregation with a detergent control.

2. **Validate computationally predicted hits experimentally**: Docking scores are not binding affinities; experimental validation is essential.

3. **Use the best available protein structure**: Docking quality depends critically on structure quality. Use high-resolution crystal structures when available.

4. **Consider protein flexibility**: Rigid docking misses many true binders; induced fit and ensemble docking improve hit rates.

5. **Profile against related proteins**: Most ligands bind multiple targets; always test selectivity against related proteins.

6. **Use large virtual libraries**: Larger libraries increase the probability of finding novel chemotypes.

7. **Determine crystal structures of hits**: X-ray crystallography of protein-ligand complexes validates binding mode and guides optimization.
