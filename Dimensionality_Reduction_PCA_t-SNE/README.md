# Dimensionality Reduction Techniques: PCA and t-SNE (Implementation from Scratch)

This repository contains the implementation of Principal Component Analysis (PCA) and t-Distributed Stochastic Neighbor Embedding (t-SNE) from scratch, showcasing key dimensionality reduction techniques, emphasizing on their mathematical foundations and practical applications.

## Dataset

The dataset used in this work is fashion_mnist1.csv, which consists of:

10,000 rows and 785 columns: Each row represents a grayscale image of a fashion item (28x28 pixels flattened into 784 features) with a corresponding label (10 classes).
The goal is to reduce the data's dimensionality for visualization and image compression while retaining meaningful information.

## Files

### 1. Principal Component Analysis `Gupta-Bonus-PCA.ipynb`
- Implements PCA using Singular-Value Decomposition (SVD).
- Tasks:
  - Decomposition of 1st and 2nd principal components and projecting data.
  - Visualizing 2D projections with color-coded labels.
  - Image compression using PCA with varying ranks (**k = 2, 5, 10**).

### 2. t-SNE (t-Distributed Stochastic Neighbor Embedding) `Gupta-Bonus-TSNE.ipynb`

- This notebook implements **t-Distributed Stochastic Neighbor Embedding (t-SNE)** from scratch using the mathematical formulation with detailed explanation.
- Key Features:
  - **Custom t-SNE Algorithm**:
    - Similarity computations (high-dimensional and low-dimensional space).
    - Gradient descent for optimizing embedding.
 - Visualize high-dimensional data in 2D by preserving local structure.
 - 2D visualization of the reduced data with labeled clusters.
  - **Hyperparameter Tuning**:
    - Evaluated five configurations, varying learning rate, perplexity, momentum, and initialization.
    - Results are assessed with metrics:
      - **D**: Distance among centroids to measure cluster separation.
      - **J**: Objective function quantifying clustering quality.
  - **Comprehensive Plots**:
    - 2D projections are visualized for each hyperparameter setting, showcasing clustering variations.


## Requirements

Ensure the following Python libraries are installed:
- **NumPy**
- **Pandas**
- **Matplotlib**
- **SVD library** (for PCA tasks)

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/eshita-ds/Data-Mining-Projects/tree/main/Dimensionality_Reduction_PCA_t-SNE
   ```
2. Open and run the Jupyter notebooks:
   - `Gupta-Bonus-PCA.ipynb`
   - `Gupta-Bonus-TSNE.ipynb`
3. Refer to markdown cells within the notebooks for detailed explanations and results.

## Insights
This work demonstrates:
- The effectiveness of PCA for linear dimensionality reduction and data compression.
- The power of t-SNE in non-linear dimensionality reduction and visualizing high-dimensional data in 2D space.
- The impact of hyperparameters on clustering and visualization outcomes.

Feel free to explore and contribute!

--------



 

  
