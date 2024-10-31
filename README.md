# BioGRNSemble-GRN-Identification
An implementation of BioGRNSemble, an ensemble machine learning methodology proposed by us that incorporates the GENIE3 and GRNBoost2 for identifying gene regulatory links between transcription factors and target genes of the Drosophila Melanogaster.

The methodology involves the following pipeline:

1. A list of 652 known transcription factors of the Drosophila is fed into GENIE3 and GRNBoost2 separately with similar hyperparameter settings.
2. Using the RNA-seq data, both models are made to predict and rank the most likely gene regulatory pairs.
3. The resulting predicted pairs of both models are then intersected to find overlapping predictions.
4. This intersection can be further trimmed down based on a minimum 'importance/correlation' score threshold.
5. TFLink, an online database of regulatory interactions between target genes and transcription factors, is used to validate the number of correct or established regulatory links. Due to the unchartered complexity of gene regulatory networks, unvalidated links can still be considered for further potential research.

## Paper:
Authors: Abdul Jawad Mohammed, Dr. Amal Khalifa
DROSOPHILA EYE GENE REGULATORY NETWORK INFERENCE USING BioGRNsemble: AN ENSEMBLE-of-ENSEMBLES MACHINE LEARNING APPROACH

BioMedInformatics 2024, 4(4), 2186-2200; https://doi.org/10.3390/biomedinformatics4040117

### Abstract/Summary: 
The paper aims to propose and demonstrate BioGRNsemble, a modular and flexible approach for inferencing gene regulatory networks from RNA-Seq data. Integrating the GENIE3 and GRNBoost2 algorithms, this ensembles-of-ensembles method attempts to balance the outputs of both models through averaging, before providing a trimmed-down gene regulatory network consisting of transcription and target genes. Using a Drosophila Eye Dataset, we were able to successfully test this novel methodology, and our validation analysis using an online database determined over 3500 gene links correctly detected, albeit out of almost 530,000 predictions, leaving plenty of room for improvement in the future.

## RNA-seq Dataset of Focus:
Potier et al. Drosophila Eye 72-sample RNA-seq expression Dataset

### Dataset Reference:
Delphine Potier, Kristofer Davie, Gert Hulselmans, Marina Naval Sanchez, Lotte Haagen, Vân Anh Huynh-Thu, Duygu Koldere, Arzu Celik, Pierre Geurts, Valerie Christiaens, Stein Aerts, Mapping Gene Regulatory Networks in Drosophila Eye Development by Large-Scale Transcriptome Perturbations and Motif Inference, Cell Reports, Volume 9, Issue 6, 2014, Pages 2290-2303, ISSN 2211-1247, https://doi.org/10.1016/j.celrep.2014.11.038. (https://www.sciencedirect.com/science/article/pii/S2211124714010043)

## Acknowledgements:
Special Thanks to Dr. Peignier, who had provided support in regards to regulatory gene prediction. A part of this code was adapted and modified from the notebooks on his website: https://sergiopeignier.github.io
