# Dimensionality Reduction Techniques: PCA and t-SNE (Implementation from Scratch)

This repository contains the implementation of Principal Component Analysis (PCA) and t-Distributed Stochastic Neighbor Embedding (t-SNE) from scratch, showcasing key dimensionality reduction techniques, emphasizing on their mathematical foundations and practical applications.

## Overview

**Dataset**

The dataset used in this work is fashion_mnist1.csv, which consists of:

10,000 rows and 785 columns: Each row represents a grayscale image of a fashion item (28x28 pixels flattened into 784 features) with a corresponding label (10 classes).
The goal is to reduce the data's dimensionality for visualization and image compression while retaining meaningful information.

**Objectives**

**1. PCA Implementation:**

- Reduce the dataset's dimensionality using Singular-Value Decomposition (SVD).
- Project data onto principal components for 2D visualization.
- Compress images using varying numbers of principal components.

**2. t-SNE Implementation:**

- Build the t-SNE algorithm from scratch using the mathematical formulation with detailed explanation.
- Visualize high-dimensional data in 2D by preserving local structure.
- Experiment with hyperparameters to evaluate their impact.

## Implementation Details

**1. Principal Component Analysis (PCA)**

**Key Steps:**

1. Data Normalization:

    - Standardize the dataset to ensure all features have zero mean and unit variance.
  
2. SVD for PCA:

    - Decompose the covariance matrix into singular vectors and values.
    - Compute the top principal components.
  
3. 2D Projection:

    - Project the data onto the first two principal components.
    - Visualize the reduced 2D data with a scatter plot, where each label (class) is represented with a different color.
  
4. Image Compression:

    - Select 10 images (one per label).
    - Compress images by retaining k=2, 5, 10 principal components.
    - Reconstruct the compressed images and compare them to the originals.
    
**Results:**
  
- **2D Scatter Plot**: Demonstrates class separability using the first two principal components.
- **Image Compression**: Visualizes how increasing the number of principal components improves the reconstructed image quality.

**2. t-SNE (t-Distributed Stochastic Neighbor Embedding)**
  
**Key Steps:** 

**1. Pairwise Similarity Computation:**

Compute the conditional probabilities P(j∣i) based on Gaussian kernels in the high-dimensional space:

  
