# Linear Regression Analysis on Coffee Shop Revenue

This project explores the application of **Simple Linear Regression**, **Multiple Linear Regression**, and **Polynomial Regression** to analyze and predict daily revenue for a coffee shop based on various features.

## Dataset

The dataset used in this analysis is `coffee_shop_revenue.csv`, which contains the following columns:

- `Number_of_Customers_Per_Day`: Number of customers visiting the coffee shop daily.
- `Average_Order_Value`: Average value of an order in dollars.
- `Operating_Hours_Per_Day`: Number of hours the shop operates daily.
- `Number_of_Employees`: Number of employees working daily.
- `Marketing_Spend_Per_Day`: Daily marketing expenditure in dollars.
- `Location_Foot_Traffic`: Foot traffic near the coffee shop's location.
- `Daily_Revenue`: Total revenue generated daily (target variable).

## Notebook Overview

The notebook `linear_regression.ipynb` implements the following:

1. **Data Preprocessing**:
   - Loading and exploring the dataset.
   - Handling missing values (if any) and scaling features.

2. **Simple Linear Regression**:
   - Analyzing the relationship between a single independent variable (e.g., `Number_of_Customers_Per_Day`) and the target variable (`Daily_Revenue`).

3. **Multiple Linear Regression**:
   - Using multiple independent variables to predict the target variable.

4. **Polynomial Regression**:
   - Extending linear regression to capture non-linear relationships between features and the target variable.

5. **Model Comparison**:
   - Comparing the performance of the three regression models using metrics such as Mean Squared Error (MSE) and R-squared.

## How to Use

1. Ensure you have the required libraries installed:
   - `pandas`
   - `numpy`
   - `matplotlib`
   - `scikit-learn`

2. Open the `linear_regression.ipynb` notebook in Jupyter Notebook or VS Code.

3. Run the cells sequentially to:
   - Load the dataset.
   - Train and evaluate the regression models.
   - Visualize the results.

## Results

The notebook provides insights into:
- The effectiveness of each regression model in predicting daily revenue.
- The impact of different features on revenue generation.
- The advantages of using polynomial regression for capturing non-linear patterns.

## Conclusion

This project demonstrates the application of regression techniques to a real-world dataset, providing a foundation for further exploration of predictive modeling in business contexts.
