# Clustering and Classification Algorithms from Scratch: K-Means, K-Means++, and KNN

## Overview
This repository focus on implementing machine learning algorithms from scratch using Python, without relying on external libraries like scikit-learn. The main objectives are to gain a deeper understanding of clustering and classification techniques.

### Dataset
The project utilizes two datasets:
1. **cluster_data1.csv**: Used for implementing and visualizing K-Means and K-Means++ clustering algorithms.
2. **cluster_data2.csv**: Used for K-Nearest Neighbors (KNN) classification.


### Key Features
1. **K-Means Clustering**
   - Implemented the K-Means clustering algorithm from scratch.
   - Visualized the centroids and cluster assignments iteratively (initial step and 4 iterations).
     <img width="557" alt="image" src="https://github.com/user-attachments/assets/36e5dd0b-585c-4809-b45a-c8346ef6b1af" />

   - Used `X1` and `X2` for 2D visualization.

2. **K-Means++ Initialization**
   - The results from the K-Means clustering algorithm are significantly influenced by the selection of centroids. Since K-Means randomly chooses initial centroids, the results can vary widely. To address this, K-Means++ was introduced. Unlike K-Means, K-Means++ selects initial centroids systematically, prioritizing diverse and distant points (step by step points shown in `Implementing_KMeans_KMeans++_KNN_from_scratch.ipynb`). After this initialization, the standard K-Means algorithm is applied, resulting in more consistent and reliable clustering outcomes.
   - Detailed comparison with K-Means:
     - K-Means++ showed better cluster formation even in the initial iteration, whereas K-Means often struggled with random centroids.
     - At iteration 4, K-Means++ delivered clear cluster distinctions, while K-Means still showed overlapping clusters.
     - Overall, K-Means++ converged faster and demonstrated the importance of effective centroid initialization.
   - Visualized the improved centroids and cluster assignments over iterations.
    <img width="552" alt="image" src="https://github.com/user-attachments/assets/9ab965c5-1c9b-4aad-8911-b2920280d4b1" />

3. **K-Nearest Neighbors (KNN) Classification**
   - Developed a KNN classifier from scratch.
   - Assigned classes to data points using results from the K-Means++ clustering.

### Detailed Solutions
The notebook provides a step-by-step implementation of each algorithm, including:
- Clear explanations of the logic behind each step.
- Code for clustering and classification.
- Iterative visualizations to track progress and results.

### Libraries Used: 
NumPy, Pandas, Matplotlib

## Files in Repository
- **Assignment Notebook**: The `Implementing_KMeans_KMeans++_KNN_from_scratch.ipynb` file contains the detailed step by step implementation and explanations.
- **Cluster Data**: Files (`cluster_data1.csv`, `cluster_data2.csv`) used for clustering and classification.

## How to Run
1. Clone the repository.
2. Install necessary libraries: `NumPy`, `Pandas`, `Matplotlib`.
3. Open the `Implementing_KMeans_KMeans++_KNN_from_scratch.ipynb` file in Jupyter Notebook.
4. Run the cells sequentially to execute the code and visualize the results.

## Results Summary
- **K-Means**: Achieved convergence in clustering with visualizations at each iteration.
- **K-Means++**: Demonstrated improved initial centroid selection, leading to better clustering.
- **KNN**: Successfully classified data points based on K-Means++ results.

## License
This project is for educational purposes only and adheres to the academic integrity policies of DATA 240.


