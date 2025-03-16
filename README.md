# Supermarket Loyalty Program Analysis

Project Overview

International Essentials is a global supermarket chain that offers a loyalty program to its customers. This program provides rewards based on annual spending, where higher spending results in bigger rewards. The supermarket aims to predict customer spending in order to estimate the cost of rewards and forecast potential profits.

Dataset Overview

The dataset contains records of customers for their last full year in the loyalty program. The key objective is to ***analyze spending patterns*** and ***determine which factors influence customer spending behavior***.

| Column Name            | Type       | Description |
|------------------------|------------|-------------|
| `customer_id`         | Integer    | Unique identifier for each customer. No missing values. |
| `spend`               | Continuous | Total amount spent by the customer in their last full year (two decimal places). Missing values replaced with `0`. |
| `first_month`         | Continuous | Amount spent by the customer in the first month of the year (rounded to two decimal places). Missing values replaced with `0`. |
| `items_in_first_month` | Discrete   | Number of items purchased in the first month. Any integer ≥ 0. Missing values replaced with `0`. |
| `region`              | Nominal    | Customer's geographic region (`Americas`, `Asia/Pacific`, `Europe`, `Middle East/Africa`). Missing values replaced with `Unknown`. |
| `loyalty_years`       | Ordinal    | Number of years the customer has been part of the loyalty program (`0-1`, `1-3`, `3-5`, `5-10`, `10+`). Missing values replaced with `0-1`. |
| `joining_month`       | Nominal    | Month the customer joined (`Jan`, `Feb`, ..., `Dec`). Missing values replaced with `Unknown`. |
| `promotion`           | Nominal    | Indicates whether the customer joined the program as part of a promotion (`Yes` or `No`). Missing values replaced with `No`. |

Problems to Solve

***Predict Customer Spending***: Develop a model to estimate how much a customer is likely to spend in the loyalty program.
***Identify Key Spending Factors***: Determine which factors (e.g., region, loyalty years, promotions) most influence total spending.
***Improve Customer Retention***: Use insights to optimize loyalty rewards and promotional strategies.

Tools & Techniques Used
***Data Cleaning & Preprocessing***
- Handled missing values using pandas.
- Converted categorical variables to ordered categories.
- Standardized inconsistent entries (e.g., promotion values standardized to 'Yes' or 'No').

***Exploratory Data Analysis (EDA)***
- Summary statistics and unique value counts.
- Data type conversion for better processing.

***Feature Engineering***
- Created categorical ordering for loyalty_years.
- Extracted insights based on spending patterns across regions and promotions.

***Baseline and Comparison Models***
- ***Baseline Model***: Linear Regression (sklearn.linear_model.LinearRegression)
  - Used first_month, items_in_first_month, and loyalty_years as features.
  - Applied OrdinalEncoder for categorical transformation.
  - Evaluated using Mean Squared Error (MSE).

- ***Comparison Model***: Random Forest Regressor (sklearn.ensemble.RandomForestRegressor)
  - Trained using 100 estimators with random_state=42.
  - Applied feature transformation for categorical encoding.
  - Compared performance using predictions on test data.

***How to Use***
***Load the datasets***: Ensure the CSV files are in the working directory.
***Run the Jupyter Notebook***: Open notebook.ipynb and execute all cells.
***Analyze Results***: Explore the findings and predictions for customer loyalty.

***Future Improvements***
Implement machine learning models for customer segmentation.
Improve data visualizations for better insights.
Integrate external factors like promotions or seasonality into the analysis.
