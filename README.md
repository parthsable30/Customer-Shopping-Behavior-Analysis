📊 Customer Shopping Behavior Analysis
An End-to-End Python + SQL + Power BI Data Analytics Project
📁 Project Overview

This project focuses on analyzing Customer Shopping Behavior using a complete data analytics workflow:

Python for data cleaning and preprocessing

SQL (MySQL) for analytical querying

Power BI for dashboard creation and business insights

The objective is to understand customer purchase patterns, revenue drivers, product performance, discount usage, and customer segmentation.

🧰 Tech Stack Used
Technology	Purpose
Python (Pandas, NumPy)	Data cleaning, preprocessing, CSV handling
SQL (MySQL)	Advanced analytics using queries, CTE, window functions
Power BI	Interactive dashboard for business insights
Matplotlib / Seaborn (optional)	Visual EDA
CSV Dataset	Raw customer behavior data

📂 Project Files in Repository
File Name	Description
customer_shopping_behavior.csv	Raw dataset
customer_shopping_behavior.ipynb
customer_shopping_behavior_dashboard.pbix	Power BI dashboard
cutomer_shopping_behavior.sql	SQL queries used for analysis
customer_shopping_behavior_project_report.pdf	Final detailed report
🔁 Workflow Summary
1️⃣ Python – Data Cleaning & Preparation

Python was used to:

Load and explore the dataset

Handle missing values

Fix inconsistent entries

Convert datatypes (age groups, numeric fields, subscription status)

Export cleaned dataset for SQL

Example Python Code Used
import pandas as pd

# Load dataset
df = pd.read_csv("customer_shopping_behavior.csv")

# Clean missing values in review ratings
df['review_rating'] = df['review_rating'].fillna(df['review_rating'].median())

# Standardize text columns
df['discount_applied'] = df['discount_applied'].str.lower()

# Export cleaned file for SQL usage
df.to_csv("customer_shopping_behavior_cleaned.csv", index=False)


2️⃣ SQL – Analytical Insights

The cleaned dataset was imported into MySQL and analyzed using advanced SQL queries.

Key SQL Analyses Performed

Revenue comparison by gender

High-spending discount users

Top-rated products

Shipping type purchase behavior

Subscribed vs Non-Subscribed Customer Spending

Top discount-utilizing products

Customer Segmentation (New, Returning, Loyal)

Top 3 products per category (Window Functions)

Repeat buyers & subscription correlation

Revenue contribution by age groups

All SQL queries are included in cutomer_shopping_behavior.sql.



3️⃣ Power BI – Dashboard & Storytelling

A professional Power BI dashboard was created to visualize:

Total revenue

Revenue by gender

Revenue by age group

Customer segmentation

Category-wise orders

Top-rated products

Discount utilization

Shipping type behavior

Subscriber vs non-subscriber performance

The dashboard helps translate raw data into actionable business insights.


📊 Key Business Insights
🔹 Revenue Insights

Age Group 25–40 contributes highest revenue.

Subscribed customers spend significantly more than non-subscribers.

🔹 Product Insights

Top-rated products indicate strong customer satisfaction.

Some categories rely heavily on discount-driven sales.

🔹 Behavioral Insights

Loyal customers (10+ previous purchases) show the highest lifetime value.

Customers choosing Express Shipping tend to spend more.

Discount users can still be high-value customers.



📌 Project Impact

This project showcases:

Real-world data cleaning using Python

Strong SQL analytics with window functions & CTEs

Business dashboard building in Power BI

Ability to extract and communicate actionable insights

Perfect for Data Analyst / BI Analyst job roles.



📜 How to Run This Project
1. Python Setup
pip install pandas numpy


Run the cleaning script to generate cleaned dataset.

2. MySQL Setup

Create a database

Import the cleaned CSV

Run queries from cutomer_shopping_behavior.sql

3. Power BI Setup

Load the cleaned CSV

Build visuals using your DAX measures and fields

Customize dashboard interactions


👤 Author

Parth Sable
Skills: Python, SQL, Power BI, Excel
