# Supermarket Loyalty Program Analysis

Project Overview

International Essentials is a global supermarket chain that offers a loyalty program to its customers. This program provides rewards based on annual spending, where higher spending results in bigger rewards. The supermarket aims to predict customer spending in order to estimate the cost of rewards and forecast potential profits.

Dataset Overview

The dataset contains records of customers for their last full year in the loyalty program. The key objective is to analyze spending patterns and determine which factors influence customer spending behavior.

Data Fields

Column Name

Type

Description

customer_id

Integer

Unique identifier for each customer. No missing values.

spend

Continuous

Total amount spent by the customer in their last full year (two decimal places). Missing values replaced with 0.

first_month

Continuous

Amount spent by the customer in the first month of the year (rounded to two decimal places). Missing values replaced with 0.

items_in_first_month

Discrete

Number of items purchased in the first month. Any integer ≥ 0. Missing values replaced with 0.

region

Nominal

Customer's geographic region (Americas, Asia/Pacific, Europe, Middle East/Africa). Missing values replaced with Unknown.

loyalty_years

Ordinal

Number of years the customer has been part of the loyalty program (0-1, 1-3, 3-5, 5-10, 10+). Missing values replaced with 0-1.

joining_month

Nominal

Month the customer joined (Jan, Feb, ..., Dec). Missing values replaced with Unknown.

promotion

Nominal

Indicates whether the customer joined the program as part of a promotion (Yes or No). Missing values replaced with No.

Problems to Solve

Predict Customer Spending: Develop a model to estimate how much a customer is likely to spend in the loyalty program.

Identify Key Spending Factors: Determine which factors (e.g., region, loyalty years, promotions) most influence total spending.

Improve Customer Retention: Use insights to optimize loyalty rewards and promotional strategies.

Tools & Techniques Used

Data Cleaning & Preprocessing: Handling missing values, categorical encoding, and data transformation.

Exploratory Data Analysis (EDA): Understanding spending trends and customer behavior.

Feature Engineering: Extracting meaningful features from available data.

Predictive Modeling: Building models to forecast customer spending and loyalty retention.

How to Use

Load the datasets: Ensure the CSV files are in the working directory.

Run the Jupyter Notebook: Open notebook.ipynb and execute all cells.

Analyze Results: Explore the findings and predictions for customer loyalty.

Future Improvements

Implement machine learning models for customer segmentation.

Improve data visualizations for better insights.

Integrate external factors like promotions or seasonality into the analysis.
