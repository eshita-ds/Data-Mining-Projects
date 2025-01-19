# A study into Food Insecurity and Resource Allocation

## 📖 Overview
"Imagine a world where millions wake up unsure if they'll have enough to eat—this is the stark reality of food insecurity. Food insecurity, the lack of reliable access to sufficient, affordable, and nutritious food, is a growing global challenge, especially as the population nears the next billion. This project delves into the key factors driving food insecurity, analyzing regional trends and patterns to uncover critical insights. At its core is the Food Insecurity Severity Index (FISI)—a composite metric designed to quantify and track global food insecurity severity, guiding impactful solutions.

## 🎯 Objective
- Identify key indicators influencing food insecurity based on four pillars: **Availability, Access, Utilization, and Stability.**
  
  <img width="600" alt="image" src="https://github.com/user-attachments/assets/f28bf03d-d3cb-44b5-be44-7fe686b61244" />
- Develop the Food Insecurity Severity Index (FISI) as a composite metric.
- Analyze trends, patterns, and anomalies in food security indicators.
- Provide region-specific recommendations for mitigating food insecurity.
- Provide actionable insights to aid policy decisions and strengthen governmental and external programs.

## 🗂️ DATA
**Source**: World Bank Development Indicators (1963-2023) [World Bank Development Indicators ](https://datacatalog.worldbank.org/search/dataset/0037712/World-Development-Indicators)

**Scope**: 1513 indicators across 217 countries; data refined to 44 indicators (2000-2020).

**Themes**: Agriculture, Economy, Health, Environment, Demographics, Education, Water & santitation, and Governance.

## ⚙️ Methodology

**Data Preprocessing:**
- Cleaned data by imputing missing values based on hierarchical strategies/predefined rules
- Addressed outliers and consolidated data for analysis (2000–2020).

**Exploratory Data Analysis:**
- Explored regional and income-group trends in cereal yields, undernourishment, and poverty.
- Analyzed the effects of extreme weather events and governance on food security over two decades (2000-2020).
  
**Feature Engineering - FISI Development:** Calculated FISI scores by aggregating weighted normalized values of indicators (0 = best security; 1 = worst insecurity).

<img width="468" alt="image" src="https://github.com/user-attachments/assets/bfce3804-141c-4ad2-a620-490379a5fd74" />

- Risk Categories:<br>
        - Low Risk (FISI ≤ 0.5),<br>
        - Medium Risk (0.5< FISI ≤ 0.63),<br>
        - High Risk (FISI > 0.63)
  
**Clustering Analysis:** Applied K-means clustering to uncover natural groupings in countries based on FISI scores and further visualized with PCA.

**Trend Analysis:** Identified expected and unexpected trends across regions.

## 🌟 Key Insights
- South Asia and Sub-Saharan Africa show the highest FISI scores, indicating severe food insecurity.
 <img width="586" alt="image" src="https://github.com/user-attachments/assets/942a7a9a-0659-4e1d-8c01-62a7c79602c5" /><br>
- Access and utilization of resources are critical; availability alone is insufficient.
- Political stability and economic strength significantly impact food insecurity levels.
- Improved food security in regions like Somalia due to effective interventions.
- Highlighted the negative impacts of political instability, climate change, and high refugee populations on food security.

## 🚀 Results
- FISI: A scalable metric categorizing countries into low, medium, and high-risk zones.
- Recommendation: Enhance agricultural productivity.
        - Focus on improving resource access and governance.
        - Mitigate risks from extreme weather and political instability.
- Visualized food insecurity trends and identified actionable insights for targeted interventions.
  
## 💡Community Contribution

- Afghanistan: To focus on creating employment opportunities to enhance GDP and improve food accessibility.
- Greece: Limit refugee intake due to resource constraints like GDP and arable land.
- South Sudan: Prioritize political stability to boost employment and food access.
- Somalia: Continue efforts in food production to transition from high to medium/low food insecurity risk.

## 🛠️ Technologies Used
- Python for data analysis and visualization.
- Machine learning for clustering and trend analysis.

## 📁 File Structure
**Folders:**
- WDI_CSV_2024_09_25 - Original Dataset extracted from World Bank Development Indicators
- staging_data - Intermediate Dataset
- ne_110m_admin_0_countries - Helper files for Geopandas mapping
- clean_data - Final Dataset ready for analysis
  
**Notebooks:**
- 1_data_collection.ipynb - This NB processes and filters World Bank country data and the indicators to extract relevant information for analysis, focusing on countries with valid region data.
- 2_EDA_beforeImputation.ipynb - This NB conducts exploratory data analysis (EDA) on global indicators, focusing on identifying patterns, outlier detection and performing univariate analysis before impuattion. 
- 3_imputation.ipynb - This NB handles missing data imputation for global indicators, applying predefined strategies. 
- 4_EDA_clean_data.ipynb - This NB conducts EDA on the clean data on global indicators, and conducted univariate analysis after impuation.
- 5_FISI_Indexes.ipynb - This notebook calculates the Food Insecurity severity index based on the 4 pillars and its corresponding indexes. Analyzed FISI over the years for trends and patterns, alongwith with deriving additional indexes.
- 6_clustering.ipynb - This NB performs clustering to uncover natural groupings in countries. Explored the clusters formed and visualised the data with PCA.
- 
**Presentation:** FoodInsecurity_project.pptx
  
## 🙌 Acknowledgements 
This project is part of the academic program supported by the **San Jose State University Department of Applied Data Science**.

Special thanks to the team members for their valuable contributions:

- Eshita Gupta
- Madhu Vishwanath Burra
- Neha Bais Thakur
- Shreya Chilumukuru

We also extend our gratitude to the **World Bank Group** for providing the dataset used in this analysis.





        
