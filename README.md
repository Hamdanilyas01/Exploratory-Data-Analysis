# Exploratory-Data-Analysis

Retail Store Sales Analysis & Discount Prediction

This project performs data cleaning, exploratory data analysis (EDA), visualization, and machine learning modeling on a retail store sales dataset.
The main goals are:

To understand sales patterns across categories, items, time, and payment methods.

To identify top-performing categories, items, and customers.

To build a machine learning model to predict whether a discount was applied on a transaction.

📂 Dataset:

File: retail_store_sales.csv

Each row represents a transaction with information such as:

Transaction ID

Customer ID

Category

Item

Price Per Unit

Quantity

Total Spent

Payment Method

Location (Online / In-store)

Transaction Date

Discount Applied (Target variable)

🧹 Data Cleaning Steps

The following preprocessing steps were applied:

Removed rows with missing Price Per Unit or Quantity.

Dropped duplicate records.

Filled missing values in Discount Applied with False.

Converted Transaction Date to datetime format.

Extracted year, month, and Month_Name from the date.

Created a YearMonth column for monthly trend analysis.

Exploratory Data Analysis:

The following visualizations were created:

1. Top 5 Categories by Total Spent

Bar chart showing the highest revenue-generating categories.

2. Top 10 Items by Total Spent

Donut chart displaying contribution of top items.

3. Total Sales by Year

Line chart showing yearly revenue trends.

4. Transactions Distribution

Donut chart showing proportion of Online vs In-store transactions.

5. Total Sales by Payment Method

Bar chart comparing total sales by Cash, Credit Card, and Digital Wallet.

6. Monthly Sales by Category

Stacked bar chart showing seasonal category performance.

7. Monthly Sales Trend

Line chart of sales aggregated by Year-Month.

8. Average Order Value (AOV) by Category

Bar chart showing average transaction value per category.

9. Top 10 Customers by Total Spent

Bar chart showing highest spending customers.

Machine Learning Model:
Objective

Predict whether a discount was applied (Discount Applied) based on transaction features.

Features Used

Category

Item

Payment Method

Location

Month

Year

Target

Discount Applied (Binary classification)

Model

Random Forest Classifier

80/20 Train-test split

5-fold Cross-validation
