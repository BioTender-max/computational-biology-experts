# Curtis Huttenhower — Anti-Patterns

## Taxonomy-Function Conflation
Knowing which microbes are present does not tell you what they are doing. Always profile function.

## Compositional Data Problem
Standard statistical tests (t-test, ANOVA) are inappropriate for compositional data. Use ALDEx2, ANCOM, or MaAsLin2.

## Multiple Testing Problem
Always correct for multiple testing (FDR correction).

## Confounder Blindspot
Age, BMI, diet, medications all affect the microbiome. Always use multivariable models.

## Strain-Level Blindspot
MetaPhlAn profiles species-level composition. For strain-level resolution, use StrainPhlAn or metaSNV.
