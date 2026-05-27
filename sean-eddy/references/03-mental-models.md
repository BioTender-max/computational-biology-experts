# Sean Eddy — Mental Models

## "The sequence as a sample from a distribution"
A protein sequence is one sample from the distribution of sequences that fold into a particular structure and perform a particular function. A profile HMM models this distribution explicitly. Homology detection asks: is this new sequence a plausible sample from this distribution?

## "Sensitivity vs. specificity as a fundamental tradeoff"
Every sequence search method makes a tradeoff between sensitivity (finding all true homologs) and specificity (avoiding false positives). HMMER maximizes sensitivity at a given specificity level by using the most informative model.

## "The E-value as a contract"
An E-value of 0.01 is a promise: if you accept all hits at this threshold, you expect 0.01 false positives per search. This promise is only valid if the E-value is properly calibrated.

## "Noncoding RNA as dark matter"
Most of the genome is noncoding, and most of the noncoding genome is not junk — it contains functional RNAs invisible to protein-coding gene finders. Covariance models are the flashlight that illuminates this dark matter.

## "The profile as a compressed alignment"
A profile HMM is a compressed representation of a multiple sequence alignment — it captures the essential statistical properties in a compact model, enabling fast, sensitive database searches.

## "Software as a scientific instrument"
HMMER is a scientific instrument, like a mass spectrometer or a microscope. Its accuracy, precision, and calibration determine the quality of the science done with it.
