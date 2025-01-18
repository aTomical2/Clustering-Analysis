# Clustering Analysis


## Overview

This repository contains a comprehensive analysis of clustering algorithms applied to a synthetic dataset. The notebook explores various clustering techniques, including K-Means and DBSCAN, and evaluates their performance under different configurations. The goal is to identify the most effective clustering approach for datasets with arbitrary shapes and varying densities.

## Features

- **Data Preprocessing**: Normalisation of dataset features for optimal clustering performance.
  
- **Clustering Algorithms**:
  - K-Means: Standard clustering method with spherical cluster assumptions.
  - DBSCAN: Density-based clustering algorithm capable of detecting arbitrarily shaped clusters and noise.

- **Visualisation**: Detailed plots of clustering results for intuitive comparison.

- **Parameter Tuning**: Exploration of parameter effects (e.g., eps in DBSCAN) on clustering outcomes.

- **Evaluation**: Comparison of clustering solutions to identify the best approach.

## Repository Structure

  - Clustering_Analysis.ipynb: The primary notebook containing code, visualisations, and analysis.
  - Sample Data: A synthetic dataset for clustering demonstrations (loaded within the notebook).
  - Outputs: Graphical comparisons of clustering results for K-Means and DBSCAN with various eps values.

## Highlights of the Analysis
- **K-Means Clustering**:
  - Produces compact, well-separated clusters.
  - Struggles with non-linearly separable clusters.
  - Less effective for datasets with arbitrary shapes.

- **DBSCAN Clustering**:
  - Tested with eps = 0.4 (dbscan1) and eps = 0.08 (dbscan2).
  - dbscan1: Over-clusters due to a high epsilon value, merging distinct clusters and adding significant noise.
  - dbscan2: Captures non-linear, arbitrary-shaped clusters effectively with a finer resolution and better noise classification.

- **Best Solution**:
  - DBSCAN with eps = 0.08 (dbscan2) outperforms K-Means and dbscan1 by adapting better to the dataset's shape and distribution while identifying noise effectively.

## Visualisations
The repository includes various plots showcasing the clustering results for each method.

## **Usage**  
- **Prerequisites**:
  - Python 3.8+
  - pandas
  - matplotlib
  - scikit-learn
  - numpy

### **Author**
**Tom Gibson**
