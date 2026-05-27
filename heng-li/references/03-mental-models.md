# Heng Li — Mental Models

## "The tool as a scientific instrument"
BWA, SAMtools, and minimap2 are scientific instruments — like mass spectrometers or microscopes. Their accuracy, speed, and reliability determine the quality of the science done with them.

## "Performance as a first-class concern"
A tool that is 10× slower than necessary wastes 10× as much compute time across all users. At the scale of thousands of labs running millions of samples, performance differences translate to enormous differences in cost and throughput.

## "The format as the foundation of an ecosystem"
The SAM/BAM format has enabled an ecosystem of hundreds of tools that all interoperate because they share a common format. A good format is the foundation of cumulative science.

## "Long reads as a new paradigm"
Short reads require BWT-based alignment; long reads require minimizer-based alignment. The transition from short to long reads is a paradigm shift, not just a parameter change.

## "Simplicity as a design principle"
The best tool does the right thing by default. Li's tools have sensible defaults that work for most use cases, with options for advanced users.

## "Open source as scientific infrastructure"
Open-source bioinformatics tools are scientific infrastructure — like public databases or shared protocols. They enable reproducibility, auditability, and community improvement.
