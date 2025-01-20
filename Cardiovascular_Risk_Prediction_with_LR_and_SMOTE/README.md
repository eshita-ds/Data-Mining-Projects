# ❤️ Binary Classification for Heart Disease Prediction using Logistic Regression

This repository implements a **Logistic Regression model** from scratch to predict the 10-year risk of coronary heart disease (CHD) using the Gradient Descent algorithm, class imbalance handling, and custom evaluation metrics.

# 📊 Key Features

**Dataset**: Cardiovascular study datasets (heart_disease_train.csv and heart_disease_test.csv).

**Task**: Predict the binary target variable TenYearCHD using **Logistic Regression built from scratch.**

**Model**: Logistic Regression with **custom implementation for gradient descent and evaluation metrics.**

<img width="180" alt="image" src="https://github.com/user-attachments/assets/dd391975-75b2-4ee2-96b4-f41e2b60b3ef" />

**Challenges Addressed:** 
  - Missing values imputed using mean/median for numerical and mode for categorical features (test data imputed based on train data to avoid leakage).
  - Severe class imbalance addressed using weighted cost functions, SMOTE, and resampling.
    
**Evaluation:**
  - Custom Gradient Descent implementation with hyperparameter tuning.
  - Custom Confusion Matrix, ROC curve plotting and AUC calculation done from scratch.

## 🧰 Methodology

**Gradient Descent:**

  - Optimized weights iteratively with a custom cost function.
    
<img width="386" alt="image" src="https://github.com/user-attachments/assets/6d2848cd-ffb2-4da1-9d72-55d52244dee6" /> 

<img width="186" alt="image" src="https://github.com/user-attachments/assets/bbfb772a-1871-472b-af93-e4eec563f990" />

  - Hyperparameters (learning rate, batch size, epochs) tuned for best accuracy, precision, recall, and AUC.
    
**Class Imbalance Handling:**

  - Weighted Cost Function: Penalized misclassification of the minority class.
  - SMOTE: Generated synthetic samples for the minority class using k-nearest neighbors.
  - Resampling: Combined oversampling (minority) and undersampling (majority).
  
**Evaluation:**

  - Plotted ROC curves and calculated AUC manually for both train and test datasets.
  - Compared baseline and improved models to highlight performance gains.

## 📈 Results and Insights

**Class Imbalance:** Addressing imbalance using weighted cost functions, SMOTE, and resampling led to:
- Better Recall (critical in healthcare applications to minimize false negatives).
- Improved AUC-ROC scores across all methods.
  
**Key Findings:**

- SMOTE: Showed improvement by generating synthetic samples but performed on par with weighted cost functions.
- Overall Model Performance: Balanced trade-off between precision and recall, with improvement in AUC and recall metrics.

## 🚀 How to Run
- Clone the repository and place the datasets (heart_disease_train.csv and heart_disease_test.csv) in the folder.
- Open `Cardiovascular_Risk_Prediction - Hyper Parameter Tuning.ipynb` or `Cardiovascular_Risk_Prediction_with_LR_and_SMOTE.ipynb` and execute cells sequentially.
