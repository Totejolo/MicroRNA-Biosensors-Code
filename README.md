# microRNA biosensors — sequence analysis

Code and data behind the figures of the preprint *MicroRNA Biosensors: Comparative Analysis and Emerging Biomedical Applications for High-Sensitivity Molecular Detection* (https://doi.org/10.6084/m9.figshare.29646443).

microRNAs are promising biomarkers for disease diagnosis because of their role in post-transcriptional gene regulation, and biosensors detect them faster and more sensitively than PCR or microarrays. This repository holds the sequence-level analysis: length and nucleotide composition of five human miRNAs commonly used as biomarkers.

## Data

`CSV` — five mature human miRNAs with their miRBase accession and sequence:

| miRNA | miRBase ID |
|---|---|
| hsa-miR-16-5p | MIMAT0000069 |
| hsa-miR-21-5p | MIMAT0000076 |
| hsa-miR-31-5p | MIMAT0000089 |
| hsa-miR-122-5p | MIMAT0000421 |
| hsa-miR-155-5p | MIMAT0000646 |

Sequences and accessions come from miRBase.

## Analysis

`Code to obtain the figures` — reads the table, computes the length of each sequence and counts the A, U, G and C bases, then produces two bar charts: sequence length per miRNA, and nucleotide composition per miRNA.

## Requirements

Python 3.9+

```
pip install pandas matplotlib
```

## Before running

The script reads a file named `a.csv`, but the data file in this repository is named `CSV`. Rename the data file to `a.csv`, or change the filename in the first lines of the script, before running it.
