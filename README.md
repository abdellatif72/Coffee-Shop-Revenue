# Coffee Shop Revenue Prediction via Linear Regression

## Project Overview

This project focuses on predicting daily coffee shop revenue using Simple, Multiple, and Polynomial Linear Regression models. Working with a dataset of 2,000 daily transaction records, the goal was to identify the most significant operational drivers of revenue—such as customer foot traffic and average order value. By rigorously evaluating feature independence and comparing multiple modeling techniques, the project successfully delivered a robust multiple linear regression model that significantly outperformed simpler baselines, offering actionable insights for coffee shop financial forecasting.

## Key Technical Steps

- **Data Cleaning:** Validated 2,000 records, identifying and removing 1 logically invalid record containing negative daily revenue to ensure data integrity.
- **Exploratory Data Analysis (EDA):** Analyzed variable relationships using `seaborn` correlation heatmaps, identifying `Number_of_Customers_Per_Day` and `Average_Order_Value` as primary revenue predictors.
- **Multicollinearity Check:** Calculated Variance Inflation Factor (VIF) using `statsmodels` to rigorously verify that the selected independent predictors did not suffer from multicollinearity.
- **Data Preprocessing:** Implemented feature scaling via `StandardScaler` from `scikit-learn` to normalize disparate feature ranges (e.g., customer counts [50-499] vs. order values [2.5-10]) and ensure equal weighting during model convergence.
- **Model Training & Selection:** Engineered and evaluated three separate models (Simple Linear, Multiple Linear, and Polynomial Degrees 2-4), analyzing the trade-offs between adding feature complexity vs. algorithmic complexity.

## Results

- Discovered that adding multiple predictive features (Multiple Linear) was vastly superior to applying higher-degree polynomial transformations (Polynomial) to a single feature.
- Built a final Multiple Linear Regression model achieving an **$R^2$ of 0.8953**, explaining nearly 90% of the variance in daily revenue.
- The Multiple Linear Regression model reduced the **Mean Squared Error (MSE) by 76.76%** (down to 105,926 from 455,703) compared to the baseline Simple Linear Regression model.
- Demonstrated that quadratic and higher-degree polynomial extensions failed to meaningfully improve upon the baseline $R^2$ of 0.5498, highlighting the linear nature of the shop's underlying economics.

## Technologies Used

- **Language:** Python 3.x
- **Data Manipulation:** `pandas`, `numpy`
- **Statistical Testing:** `statsmodels` (VIF Analysis)
- **Machine Learning:** `scikit-learn` (LinearRegression, PolynomialFeatures, StandardScaler, model evaluation metrics)
- **Visualization:** `matplotlib`, `seaborn`
