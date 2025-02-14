# Mental Health Clustering Based on Tech Jobs

## Overview

This repository contains the project "Mental Health Clustering based on Tech Jobs," conducted as a case study for the course DLBDSMLUSL01 - Machine Learning: Unsupervised Learning and Feature Engineering.

The study aims to analyze survey data from employees in technology roles to identify clusters based on mental health responses. The goal is to provide actionable insights for Human Resources (HR) to design targeted mental health initiatives, fostering a healthier workplace environment.

## Table of Contents

1. [Introduction](#introduction)
2. [Methodology](#methodology)
   - [Tools and Libraries](#tools-and-libraries)
   - [Simplifying](#simplifying)
   - [Removing Outliers](#removing-outliers)
   - [Remapping](#remapping)
   - [Handling Missing Values](#handling-missing-values)
   - [Dropping Columns](#dropping-columns)
   - [Encoding the Dataset](#encoding-the-dataset)
   - [Data Scaling](#data-scaling)
   - [Dimensionality Reduction](#dimensionality-reduction)
   - [Clustering](#clustering)
3. [Results and Conclusion](#results-and-conclusion)
4. [References](#references)
5. [Appendices](#appendices)

## Introduction

The study analyzes survey data from employees in technology roles to identify clusters based on mental health responses. The goal is to provide actionable insights for HR to design targeted mental health initiatives, fostering a healthier workplace environment.

## Methodology

### Tools and Libraries

- **Pandas:** Reading, cleaning, and manipulating the dataset
- **NumPy:** Handling arrays and data frame operations
- **Matplotlib & Seaborn:** Visualizing and plotting data
- **Scikit-learn (Sklearn):** Various preprocessing and clustering tools
- **UMAP:** Dimensionality reduction
- **Yellowbrick:** Elbow method for determining the optimal number of clusters
- **KMeans:** Clustering algorithm

### Simplifying

- Renamed columns to concise and descriptive formats
- Converted text data to lowercase and removed extra spaces

### Removing Outliers

- Removed unrealistic age values (below 18 and above 80)

### Remapping

- Standardized ambiguous responses
- Simplified binary responses for consistency
- Unified multilevel categorical responses
- Standardized gender data

### Handling Missing Values

- Replaced missing values in numerical columns with the median
- Imputed missing values in categorical features with the most frequent category

### Dropping Columns

- Removed columns with high cardinality that complicated the analysis

### Encoding the Dataset

- Applied various encoding strategies (binary encoding, ordinal encoding, multi-label binarization, frequency encoding)

### Data Scaling

- Used `StandardScaler` to standardize the features

### Dimensionality Reduction

- Applied UMAP for better separation of data points

### Clustering

- Determined optimal clusters using the elbow method
- Applied KMeans for clustering
- Evaluated clusters using metrics such as Silhouette Score, Calinski-Harabasz Score, and Davies-Bouldin Score

## Results and Conclusion

The KMeans clustering algorithm identified four distinct clusters, each representing unique mental health characteristics. These insights can help HR design targeted mental health programs tailored to employees' needs.

## References

- Venkatesh, D. (2016). Mental health in tech survey 2016 [Data set]. Open Sourcing Mental Illness. [Kaggle](https://www.kaggle.com/osmi/mental-health-in-tech-2016)

## Appendices

- Detailed graphs and code available in the full repository: [GitHub](https://github.com/NasiriMohsen/Unsupervised-Learning-Mental-Health-Dataset)

