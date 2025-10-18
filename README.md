# House-Price-Analysis-using-Linear-Regression-and-XGBoost

## Overview
This repository contains a comprehensive technical assessment focused on predicting house sale prices using a real-world dataset. The project demonstrates a complete machine learning workflow, from initial Data Cleaning and Exploratory Data Analysis (EDA) to advanced Feature Engineering, Model Training (XGBoost), and rigorous Evaluation.

The primary goal was to build an accurate predictive model and provide a concise, mixed technical/non-technical summary of the findings and the most impactful features.

## Project Workflow
The analysis is documented end-to-end in the House_Price_Assessment.ipynb Jupyter Notebook and includes the following steps:

- Data Cleaning: Handled missing values, detected and managed duplicates, and ensured consistency across temporal features (e.g., YearBuilt).

- Exploratory Data Analysis (EDA): Analyzed feature distributions, identified correlations between key variables and the target variable (SalePrice), and addressed significant outliers.

- Feature Engineering: Created new features (like HouseAge), encoded categorical variables (One-Hot Encoding), and normalized numeric features to prepare the data for modeling.

- Modeling:

      Trained a baseline Linear Regression model for comparison.

      Developed a high-performance XGBoost Regressor model.

- Evaluation: Compared model performance using key metrics: Root Mean Squared Error (RMSE) and R² (Coefficient of Determination).

- Hyperparameter Tuning & Feature Impact: Optimized the XGBoost model using techniques like Grid Search and analyzed feature importance to understand model drivers.


## Key Results and Model Performance
The XGBoost Regressor was selected as the final model due to its superior performance and ability to capture complex, non-linear relationships in real estate data.

| Model             |   RMSE (Original Scale) |   $R^{2}$ Score (Log Scale) |
|:------------------|------------------------:|----------------------------:|
| Linear Regression |                 88465.1 |                      0.7571 |
| XGBoost           |                 81970.8 |                      0.7774 |



## Top 5 Influential Features
Based on the XGBoost feature importance analysis, the following factors were found to have the greatest impact on the predicted house price:

1. OverallQual (Overall Quality): Material and finish quality is the most critical factor.

2. GrLivArea (Above Grade Living Area): Total square footage of living space.

3. Neighborhood: The specific location/desirability of the neighborhood.

4. TotalBsmtSF (Total Basement Square Feet): Size of the basement area.

5. GarageCars: Capacity of the garage.



