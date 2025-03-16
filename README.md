# Supermarket Loyalty Program Analysis

Project Overview

This project analyzes customer loyalty program data for a supermarket chain to understand purchasing behavior and factors affecting customer spending. The analysis helps in predicting customer retention and optimizing promotional strategies.

Dataset Overview

The project uses multiple datasets, including:

loyalty.csv: Contains customer spending, first purchase details, regional information, and promotional data.

train.csv: Training data for predictive modeling, includes spending patterns and loyalty duration.

test.csv: Data used for testing model performance.

validation_loyalty.csv: Used for model validation.

Key Features in the Dataset:

customer_id: Unique identifier for each customer.

spend: Total amount spent.

first_month: Spending amount in the first month.

items_in_first_month: Number of items purchased in the first month.

region: Customer's geographical location.

loyalty_years: Years the customer has been in the loyalty program (categorized).

joining_month: Month the customer joined the program.

promotion: Indicates whether the customer was part of a promotional campaign.

Tools & Techniques Used

Data Cleaning & Preprocessing

Handled missing values using pandas.

Converted categorical variables to ordered categories.

Standardized inconsistent entries (e.g., promotion values standardized to 'Yes' or 'No').

Exploratory Data Analysis (EDA)

Summary statistics and unique value counts.

Data type conversion for better processing.

Feature Engineering

Created categorical ordering for loyalty_years.

Extracted insights based on spending patterns across regions and promotions.

Predictive Modeling (if applicable)

The dataset structure allows for potential customer retention modeling using regression or classification.

Key Insights

Customers with higher loyalty years tend to spend more.

Customers in certain regions show higher spending trends.

Promotional campaigns have a mixed impact on customer retention.

How to Use

Load the datasets: Ensure the provided CSV files are in the working directory.

Run the Jupyter Notebook: Open notebook.ipynb and execute all cells.

Explore insights: The notebook will display data summaries, visualizations, and potential model predictions.

Future Improvements

Implement predictive modeling to classify loyal vs. non-loyal customers.

Visualize spending patterns using matplotlib/seaborn.

Integrate more customer demographics for enhanced analysis.
