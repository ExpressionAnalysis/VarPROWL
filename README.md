# VarPROWL
Variant PROfiling with Logistic Regression

## Description
VarPROWL performs an in-depth analysis of each nucleotide position, in an effort to accurately identify variants.  VarPROWL examines a multitude of metrics before making a call.  These metrics/calculations include:

* Context specific error – each sequencing platform, chemistry, and kit have their own unique properties, and in some cases, may have systematic, context-specific errors associated with them which may result in erroneous variant calls, if not identified.

* Bidirectionality – aside from explicitly identifying systematic, context specific errors, another way to identify erroneous variant calls is to ensure that you have coverage on both strands, and that the putative variant is present on both.

* Error rate modeling – Sequencing error rates of forward and reverse reads are estimated independently using a logistic regression model which results in more accurate error modelling compared to Illumina’s average base quality, alone.

Variants are output in VCF v 4.2 (Variant Call Format).

# Citations
- Brown C, et al. “Detecting low frequency SNVs with NGS sequencing - Introducing VarPROWL.” 22nd Annual International Conference on Intelligent Systems for Molecular Biology, Boston, MA, USA. 2014
