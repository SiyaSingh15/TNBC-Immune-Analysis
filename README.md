# Immune Activation Analysis in Triple-Negative Breast Cancer (TNBC)

## Overview

This project investigates immune activation patterns in breast cancer tumors using publicly available gene expression data. The goal was to quantify tumor immune activity, compare immune levels across subtypes, discover immune subgroups, and evaluate whether immune gene expression can predict TNBC status.

## Dataset

Gene expression data were obtained from the GEO database (GSE45827), containing breast tumor samples with subtype annotations.

## Methods

### 1. Gene Mapping

Microarray probe identifiers were mapped to gene symbols using the GPL570 platform annotation.

### 2. Immune Gene Panel

A curated panel of cytotoxic immune activation genes was selected, including markers of T-cell activity, interferon signaling, and immune checkpoints.

### 3. Immune Score Calculation

For each tumor sample, immune activity was quantified as the mean standardized expression of the immune gene panel.

### 4. Subtype Comparison

Immune scores were compared between TNBC and other breast cancer subtypes using visualization and a Mann-Whitney U statistical test.

### 5. Heatmap Visualization

Hierarchical clustering of immune gene expression revealed heterogeneous immune activation patterns across tumors.

### 6. Unsupervised Clustering

K-means clustering identified immune-high and immune-low tumor groups directly from gene expression data.

### 7. Machine Learning Prediction

A logistic regression classifier was trained to predict TNBC status from immune gene expression. The model achieved strong predictive accuracy, demonstrating that immune signatures contain meaningful subtype information.

## Key Findings

* TNBC tumors tend to show higher immune activation than other breast cancers.
* Tumors exhibit substantial heterogeneity, with both immune-high and immune-low subgroups.
* Immune gene expression alone can predict TNBC status with good accuracy.

## Tools Used

* Python
* pandas
* seaborn
* scikit-learn
* matplotlib

## Author

Siya Singh
IISER Tirupati
(Student bioinformatics project)

