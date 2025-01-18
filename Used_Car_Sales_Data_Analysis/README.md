# Used Car Sales Data Analysis

This repository contains a Jupyter Notebook that explores and analyzes a dataset of used car sales. The notebook provides detailed insights into the dataset, including data cleaning, feature engineering, and exploratory data analysis (EDA). It also includes mathematical explanations and reasoning for the chosen approaches to better understand the data and derive meaningful conclusions. The goal of this analysis is to uncover key insights into factors affecting used car prices and to clean, transform, understand, and analyze the data effectively.

## Key Features

**1. Data Cleaning**

- Removed unnecessary columns (`S.No, New_Price`) to focus on relevant data.
- Created a new feature `Car_Age` by calculating the difference between the current year and the year of manufacture.
- Addressed missing values in critical columns (`Mileage, Engine, Power, Seats`) using logical imputation:
  - Subgroup-based imputation (e.g., filling missing Seats based on car type). <br>
  - Internet research to estimate reasonable values for electric vehicles' mileage.

**2. Data Transformation**

- Converted object-type columns (`Mileage, Engine, Power`) into numerical formats by removing units and standardizing values (e.g., converting km/kg to kmpl).
- Ensured consistency in units across all records for better analysis.
- Documented each transformation step with clear reasoning and references.
  
**3. Outlier Detection**

- Checked data distribution (normal vs. non-normal) for numerical columns like Car_Age, Kilometers_Driven, Mileage, etc.
- Based on the data distribution type, detected outliers using statistical methods:
  - For normal distributions: Used z-scores.
  - For non-normal distributions: Applied interquartile range (IQR).
- Visualized outliers using box plots to identify anomalies effectively.
  
**4. Correlation Analysis**
- Calculated Pearson correlation coefficients between key numerical features (‘Car_Age’, ‘Kilometers_Driven’, ‘Mileage’, ‘Engine’, ‘Power’, ‘Seats’, ‘Price’) after excluding outliers.
- Understanding Person Correlation coefficient Heatmap to identify strong/Moderate/weak/Negative correlations with target.
- Visualized correlations using scatter plots with coefficient values embedded in the figures.
- Observed strong negative correlation between car age and price, indicating depreciation trends.
  
**5. Handling Missing Values**
- Counted missing values in key columns (Mileage, Engine, Power, etc.) and treated them as follows:
  - Subgroup-based imputation for categorical/discrete features (e.g., mode for seats).
  - **Linear regression models** to predict missing values in continuous features (Mileage, Price) based on correlated attributes.
- Visualized imputed data using histograms with distinct colors for original and imputed values.

## Approach Highlights

The notebook emphasizes transparency and reasoning at every step:

Why This Over That? Each decision—be it imputation method or transformation technique—is supported by logical reasoning or mathematical justification.

Mathematical Explanations: Includes calculations for correlation coefficients, regression models, and outlier thresholds to ensure robust analysis.

Human-Centric Progress: The notebook reflects significant strides in understanding the dataset, with clear documentation of challenges faced and solutions implemented.

## **Conclusion**

This notebook reflects substantial progress in analyzing the used car sales dataset. By combining thoughtful data cleaning, feature engineering, EDA, and mathematical reasoning, it provides actionable insights into factors influencing car prices. The structured approach ensures clarity and reproducibility for future analyses.
