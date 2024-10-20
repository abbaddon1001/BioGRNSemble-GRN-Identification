# BioGRNSemble-GRN-Identification
An implementation of BioGRNSemble, a proposed ensemble machine learning methodology incorporating the GENIE3 and GRNBoost2 for identifying gene regulatory links between transcription factors and target genes of the Drosophila Melanogaster.

## Authors: Abdul Jawad Mohammed, Dr. Amal Khalifa

Original Thesis Paper: https://hammer.purdue.edu/articles/thesis/Inferencing_Gene_Regulatory_Networks_for_Drosophila_Eye_Development_Using_an_Ensemble_Machine_Learning_Approach/25686468?file=45993024

## Abstract: 
The paper aims to propose and demonstrate BioGRNsemble, a modular and flexible approach for inferencing gene regulatory networks from RNA-Seq data. Integrating the GENIE3 and GRNBoost2 algorithms, this ensembles-of-ensembles method attempts to balance the outputs of both models through averaging, before providing a trimmed-down gene regulatory network consisting of transcription and target genes. Using a Drosophila Eye Dataset, we were able to successfully test this novel methodology, and our validation analysis using an online database determined over 3500 gene links correctly detected, albeit out of almost 530,000 predictions, leaving plenty of room for improvement in the future.

## Dataset of Focus:
Potier et al. Drosophila Eye 72-sample RNA-seq expression Dataset

## Dataset Reference:
Delphine Potier, Kristofer Davie, Gert Hulselmans, Marina Naval Sanchez, Lotte Haagen, Vân Anh Huynh-Thu, Duygu Koldere, Arzu Celik, Pierre Geurts, Valerie Christiaens, Stein Aerts, Mapping Gene Regulatory Networks in Drosophila Eye Development by Large-Scale Transcriptome Perturbations and Motif Inference, Cell Reports, Volume 9, Issue 6, 2014, Pages 2290-2303, ISSN 2211-1247, https://doi.org/10.1016/j.celrep.2014.11.038. (https://www.sciencedirect.com/science/article/pii/S2211124714010043)

## Acknowledgements:
Special Thanks to Dr. Peignier, who had provided support in regards to regulatory gene prediction. A part of this code was adapted and modified from the notebooks on his website: https://sergiopeignier.github.io
