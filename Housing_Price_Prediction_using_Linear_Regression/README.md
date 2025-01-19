# 🏠 House Price Prediction using Linear Regression

This repository implements a **Linear Regression model from scratch** to predict housing prices in Windsor, Ontario, Canada. The focus is on building a solid understanding of the Gradient Descent algorithm by implementing it manually and optimizing weights for the model.

## 📊 Key Features

- **Dataset**: Housing sales prices (housing.csv) from Windsor, Ontario, with multiple variables influencing the target variable `price`.
  
- **Model**: Linear Regression with multivariate input features.
  
- **Optimization**: Two Gradient Descent algorithms:
  - Part 1.1: Scalar-based calculations for cost minimization.
  - Part 1.2: Matrix-based computations for efficient optimization.
    
- **Performance Metrics:**
   - Root Mean Squared Error (RMSE) for iterative progress tracking.
   - R² Score for model performance evaluation.
 
## 🧰 Methodology

**💡 Gradient Descent in Linear Regression**

The objective of linear regression is to minimize the cost function. Gradient Descent is an optimization algorithm that minimizes the cost function by iteratively adjusting the model's weights. The process ensures that the predicted values (𝑦^) approach the true target values (𝑦).

**1. Cost Function (MSE):**

  <img width="226" alt="image" src="https://github.com/user-attachments/assets/e35f952e-79ce-41b8-ab64-cdc9aa1e1452" />  <img width="264" alt="image" src="https://github.com/user-attachments/assets/5888f779-89e4-4a0e-aea7-706db5923b6f" />

  <img width="221" alt="image" src="https://github.com/user-attachments/assets/bd555fe2-6ca1-4965-8d18-dd742b410dce" />

  Here, 𝐽 measures the error between predicted and actual values.

**2. Weight Updates:** Using partial derivatives of the cost function:

<img width="269" alt="image" src="https://github.com/user-attachments/assets/4c335067-11c7-41a7-af50-bc9b018332d4" />

- α: Learning rate (step size).
- <img width="53" alt="image" src="https://github.com/user-attachments/assets/315527da-8c59-407a-af20-41ebd12c166f" /> : Gradient of the cost function with respect to weight 𝑊𝑗.

**3. Feature Scaling:** To improve convergence speed, input features are normalized using mean normalization or z-score normalization.

## ⚙️ Implementation Details

**Part 1.1: Scalar-Based Gradient Descent**

- Iteratively updates weights based on individual feature contributions.
- Tracks RMSE across 10 epochs.
- Visualized `True Price` vs `Predicted Price` and evaluated 𝑅^2.

**Part 1.2: Matrix-Based Gradient Descent**

 - Utilizes matrix algebra for simultaneous updates across features.
 - Optimizes cost using
   
  <img width="198" alt="image" src="https://github.com/user-attachments/assets/e6c87d7b-580d-45de-8f5c-c984a724c0c0" />
 
  ∇ W: Gradient vector, computed for all weights simultaneously.

## 📈 Key Results
- **Convergence:** RMSE steadily decreased across iterations, confirming effective optimization.
- **Performance:**
  - Achieved a strong 𝑅^2 score, reflecting accurate predictions.
  - Visual plots validate alignment between actual and predicted prices

    <img width="438" alt="image" src="https://github.com/user-attachments/assets/2e972759-4ef7-4759-b4ec-68a29a7a8f51" /> <img width="423" alt="image" src="https://github.com/user-attachments/assets/ffc66cf6-6ade-41c9-94f8-5c4bf4e44783" />

## 🚀 How to Run
- Clone the repository.
- Download housing.csv and place it in the project folder.
- Run the Jupyter Notebook `Housing Price Prediction using Linear Regression.ipynb` step-by-step.



