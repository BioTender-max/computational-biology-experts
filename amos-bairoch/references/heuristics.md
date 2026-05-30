## Key heuristics

- Always use UniProt/Swiss-Prot reviewed entries (evidence level:
  experimental) as the gold standard for protein function annotation.
  TrEMBL entries are starting points, not conclusions.
- When building a biological database, define the controlled vocabulary
  before writing the first entry. Retrofitting vocabulary to existing
  entries is extremely costly.
- Cite the primary literature for every annotation. "Inferred from
  homology" is a valid evidence code, but it must be stated explicitly.
- Cross-link to all relevant databases (PDB, OMIM, GO, KEGG) from every
  entry. Isolated databases are less useful than connected ones.
- Version every database release. Users need to know which version of
  Swiss-Prot their analysis used.

---