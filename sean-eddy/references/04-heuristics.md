# Sean Eddy — Heuristics

1. Use profile HMMs, not BLAST, for sensitive homology detection — HMMER is more sensitive at the same specificity.
2. Report E-values, not bit scores or percent identity — E-values have statistical meaning.
3. Use the forward algorithm, not Viterbi, for scoring — forward is more sensitive.
4. Search Rfam before annotating noncoding regions — many "unknown" regions contain known RNA families.
5. Use covariance models for RNA — sequence-only methods miss RNA families with compensatory mutations.
6. Calibrate your E-values — don't trust tools that don't report calibrated E-values.
7. Train profile HMMs on curated seed alignments — garbage in, garbage out.
8. Use hmmscan for domain annotation, hmmsearch for database search — different use cases, different commands.
9. Check for remote homologs before calling a protein "novel" — HMMER finds homologs that BLAST misses.
10. Use Pfam for protein domain annotation — it's the most comprehensive and curated database.
11. Don't confuse statistical significance with biological significance — a significant E-value is a hypothesis, not a fact.
12. Use iterative searches (jackhmmer) for very remote homologs — like PSI-BLAST but probabilistically correct.
13. Validate computational predictions with experimental evidence — sequence analysis is hypothesis generation.
14. Read the HMMER user guide — it explains the statistics better than most textbooks.
15. Use --cut_ga, --cut_tc, or --cut_nc thresholds for Pfam/Rfam — these are curated gathering thresholds.
16. Don't use percent identity as a homology criterion — it's not statistically calibrated.
17. Consider secondary structure when analyzing RNA — sequence conservation alone is insufficient.
18. Use multiple sequence alignments as input to profile building — more sequences = better model.
19. Be skeptical of "novel" proteins — most have remote homologs detectable by HMMER.
20. Publish your models — a profile HMM is a scientific contribution that others can use.
