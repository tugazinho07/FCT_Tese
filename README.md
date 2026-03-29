# FCT_Tese

# Metagenomic Binning Under Limited Data Conditions

This repository contains the code and scripts developed as part of a Master's dissertation focused on evaluating metagenomic binning performance under constrained data scenarios.

## Overview

Metagenomic binning is a key step in reconstructing microbial genomes from sequencing data. Most existing benchmarking studies assume access to large, high-quality datasets. This work investigates how binning performance is affected when the amount of available data is reduced.

The main goal is to evaluate whether alternative strategies such as multi-sample binning and co-assembly can compensate for limited input data.

## Repository Contents

This repository includes:

- Scripts for data preprocessing (assembly, filtering, preparation)
- Execution scripts for binning tools:
  - MetaBAT
  - SemiBin
  - MetaBinner
  - COMEBin
- Workflow automation for running experiments across:
  - Single-sample
  - Multi-sample
  - Co-assembly configurations
- Result aggregation and formatting scripts
- Supporting files for reproducing figures and tables

## Datasets

The experiments were conducted using:

- Cheese fermentation datasets (short-read)
- Activated sludge datasets (long-read)

Public datasets were obtained from NCBI repositories.

## Key Findings

The results show that reducing the dataset size to six samples leads to a significant decrease in binning performance:

- Between **17% and 68%** of high-quality genome bins were recovered compared to the reference study
- Co-assembly provided the best performance under limited data conditions
- Multi-sample binning showed reduced effectiveness when fewer samples were available

## Reproducibility

All experiments can be reproduced using the scripts provided in this repository. The workflow is designed to be modular, allowing adaptation to different datasets or additional binning tools.

- Linux environment (tested on HPC cluster)
- Standard bioinformatics tools:
  - Samtools
  - MEGAHIT
- Binning tools:
  - MetaBAT
  - SemiBin
  - MetaBinner
  - COMEBin

Gonçalo Soares 67544

Developed as part of a Master's thesis at NOVA FCT.

Master Thesis Computer Science

This project is intended for academic and research purposes.
