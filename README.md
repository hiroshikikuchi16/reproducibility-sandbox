# README
Based on the provided R Markdown code, here's a comprehensive README file that describes the Acute Myeloid Leukemia Heatmap analysis:

# Acute Myeloid Leukemia Heatmap Analysis

## Overview

This repository contains an RNA-seq analysis pipeline focused on acute myeloid leukemia (AML) samples. The analysis generates clustering heatmaps to visualize gene expression patterns across different AML mutations and treatments.

## Dataset Description

- Source: Shih et al., 2017 study (PubMed ID: `28193779`)
- Platform: RNA-seq data from refine.bio
- Samples: 19 AML model mice samples
- Processing: Quantile normalized data
- Access: Available through refine.bio experiment SRP070849

## Analysis Pipeline

Data Organization- Creates structured directory system for data, plots, and results
- Manages sample metadata and expression data

Data Processing- Reads TSV files containing gene expression data
- Performs variance-based gene selection
- Filters genes in upper quartile of variance

Heatmap Generation- Creates annotated heatmaps using pheatmap
- Includes sample clustering analysis
- Visualizes treatment effects and mutations

## Key Features

- Reproducible analysis pipeline
- Sample clustering visualization
- Treatment effect comparison
- Mutation status tracking
- Automated directory management

## Requirements

- R environment
- Required packages:
  - pheatmap
  - magrittr
  - readr
  - tibble
  - dplyr
  - sessioninfo



## Usage Instructions

Clone the repositoryDownload the dataset from refine.bio (SRP070849)Place the downloaded files in the data directoryRun the analysis pipelineResults will be generated in the plots and results directories## Output Files

- Heatmap visualization (PNG format)
- Filtered gene expression data (TSV format)
- Session information report

## Citations

- Original analysis adapted from refine.bio-examples notebook
- Dataset source: Shih et al., 2017 (PubMed ID: 28193779)
- Visualization methods based on pheatmap package documentation