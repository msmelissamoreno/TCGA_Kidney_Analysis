# TCGA Kidney Cancer RNA-seq Classification Using NSGA-II

This repository contains the Google Colab notebooks used for an RNA-seq classification analysis of the three major renal cell carcinoma cohorts in The Cancer Genome Atlas (TCGA): kidney chromophobe (KICH), kidney renal clear cell carcinoma (KIRC), and kidney renal papillary cell carcinoma (KIRP).

The analysis applies a multi-objective NSGA-II feature selection framework to identify parsimonious gene subsets that retain strong discriminatory performance in a high dimensional transcriptomic dataset. Candidate gene subsets are evaluated during feature selection using cross validated balanced accuracy and a parsimony objective. Genes selected by NSGA-II are subsequently supplied to a single interpretable decision tree classifier, which is evaluated on an independent held-out validation cohort.

Parallel analyses using transcripts per million (TPM) and counts per million (CPM) normalization were performed to examine whether RNA-seq normalization influences gene selection, classifier structure, and held-out predictive performance.

The repository includes notebooks for data retrieval and preprocessing, NSGA-II feature selection, final decision tree development, validation performance assessment, feature importance, and exploratory survival analyses.
