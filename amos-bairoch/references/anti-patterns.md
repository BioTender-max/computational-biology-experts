# Anti-Patterns — Amos Bairoch

## 1. Quantity Over Quality

**The pattern**: Maximizing entry count at the expense of annotation depth. Racing to include as many sequences as possible while providing only shallow, unverified annotations.

**Why it fails**: A database with 10 million shallow entries is less useful than one with 100,000 deeply annotated entries. Shallow annotations cannot support the downstream analyses — functional prediction, drug target identification, disease gene interpretation — that make protein databases valuable. Errors in shallow annotations propagate through the literature and into automated pipelines, compounding over time.

**Bairoch's response**: Swiss-Prot deliberately maintained a curated, non-redundant core even as TrEMBL grew to contain orders of magnitude more entries. The two-tier architecture was a principled solution: provide coverage (TrEMBL) without compromising quality (Swiss-Prot). The "Swiss clock" standard was non-negotiable.

**The temptation**: Funding bodies and users often measure databases by entry count. The pressure to show growth in numbers can drive teams toward quantity at the expense of quality. Resisting this pressure requires institutional commitment to quality as the primary metric.

---

## 2. Treating Databases as Finished Projects

**The pattern**: Building a database, releasing it, and then assuming it can be maintained with minimal ongoing effort. Treating annotation as a one-time activity rather than a continuous process.

**Why it fails**: Biological knowledge is not static. New experimental results continuously revise our understanding of protein function, structure, and disease associations. A database that is not continuously updated becomes outdated and unreliable — and because researchers trust databases, outdated information can mislead research for years.

**Bairoch's experience**: He originally planned to hand Swiss-Prot off to EMBL after completing his PhD. The rapid growth of protein sequence data made this impossible — Swiss-Prot required continuous, intensive curation effort that grew with the database. He ended up dedicating decades to its development.

**The staffing implication**: Databases require permanent staff, not rotating postdocs and students. The institutional knowledge accumulated by long-term annotators — some Swiss-Prot annotators stayed for 15 years — is irreplaceable. High turnover destroys annotation consistency and quality.

---

## 3. Automation Without a Gold Standard

**The pattern**: Deploying automated annotation pipelines without a high-quality manually curated reference set to propagate from. Using machine learning or rule-based systems to annotate proteins without validating against a trusted manual reference.

**Why it fails**: "You cannot propagate something that does not exist." Automated pipelines can scale annotation, but they can only propagate what exists. Without a gold standard, automated annotation propagates errors and uncertainties at scale. The result is a large volume of plausible-looking but unreliable annotations that are difficult to distinguish from accurate ones.

**The compounding problem**: Errors in automated annotations are often cited in papers, which then become sources for further automated annotation. The error propagates through the literature and into other databases, becoming increasingly difficult to trace and correct.

**Bairoch's solution**: The HAMAP pipeline for bacterial and archaeal proteins was built on a foundation of Swiss-Prot entries. It is "probably one of the most reliable automatic annotation pipelines operationally deployed" precisely because it propagates from a high-quality manual reference. The manual gold standard is not a bottleneck — it is the prerequisite for reliable automation.

---

## 4. Siloed Resources

**The pattern**: Building databases that do not cross-reference other relevant resources. Creating isolated knowledge silos that require users to manually transfer information between systems.

**Why it fails**: Biological knowledge is inherently interconnected. A protein's sequence, structure, function, disease associations, pathway context, and organism-specific biology are all related. A database that provides only one of these dimensions forces users to manually integrate information from multiple sources, introducing errors and missing connections that would be visible in an integrated system.

**Bairoch's response**: Every resource he built was tightly integrated with others. Swiss-Prot entries cross-reference ~100 external databases. ExPASy tools read Swiss-Prot annotations to enhance their predictions. InterPro unified PROSITE, PRINTS, BLOCKS, PRODOM, and Pfam. neXtProt extended Swiss-Prot human annotation with proteomics, expression, and variant data.

**The institutional obstacle**: Siloed databases are often driven by institutional incentives that reward novelty over interoperability. Building a new database is more publishable than integrating with existing ones. Overcoming this requires deliberate effort and, often, formal collaboration agreements.

---

## 5. Ignoring Nomenclature

**The pattern**: Failing to develop or adopt controlled vocabularies and nomenclature standards. Using free-text descriptions for biological entities that should be represented by standardized terms.

**Why it fails**: Without standardized terminology, databases cannot be queried consistently, tools cannot interoperate, and knowledge cannot be aggregated across resources. The same protein may be described as "kinase," "protein kinase," "serine/threonine kinase," and "STK" in different databases — making it impossible to retrieve all relevant information with a single query.

**Bairoch's observation**: "You will always wonder why life scientists abhor complying with nomenclature guidelines or standardisation efforts that would simplify your and their life." Despite this resistance, he consistently pushed for standardization, arguing that the short-term inconvenience of adopting standards is far outweighed by the long-term benefits of interoperability.

**The ENZYME database**: Created specifically to provide a standardized repository for enzyme nomenclature, based on the IUBMB recommendations. It became an indispensable resource for metabolic databases precisely because it provided a controlled vocabulary for enzyme function.

---

## 6. Funding Infrastructure as Research

**The pattern**: Applying short-term research grant logic to long-term infrastructure. Funding databases through 2–5 year grants that require constant renewal and create uncertainty about continuity.

**Why it fails**: Databases need stable, multi-decade funding. The 2–5 year grant cycle creates several problems:
- Uncertainty about continuity discourages long-term staff commitments
- Grant renewal requires demonstrating novelty, which conflicts with the maintenance-focused nature of database work
- Gaps between grants can cause loss of staff and institutional knowledge
- The pressure to show new results drives teams toward adding new features rather than maintaining existing ones

**Bairoch's experience**: Swiss-Prot nearly closed in 1996 when European and Swiss funding simultaneously fell through. The crisis was resolved only through emergency funding and the creation of SIB as an institutional solution. "We are a pain in the neck for funding bodies: we require long-term solutions and not 2 to 5 years research grants."

**The institutional solution**: The Swiss Institute of Bioinformatics was created to provide stable, long-term funding for bioinformatics infrastructure. It operates under a constitutional provision that authorizes the Confederation to finance non-profit research of national interest — a model that decouples infrastructure funding from the grant cycle.
