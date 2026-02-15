#  Customer Shopping Behavior Analytics Dashboard

An end-to-end Business Intelligence project analyzing customer
purchasing behavior using **Python, MySQL, SQL, and Power BI** to
generate actionable business insights.

------------------------------------------------------------------------

## 📌 Project Overview

This project analyzes retail customer shopping behavior to identify
revenue drivers, subscription trends, discount effectiveness, product
performance, and customer segmentation patterns.

### BI Workflow:

-   Data Cleaning & Feature Engineering (Python -- Pandas)
-   Database Storage & Querying (MySQL)
-   Advanced SQL Analysis
-   Interactive Dashboard Development (Power BI)
-   Business Insight Generation

------------------------------------------------------------------------

## 🏗️ Project Architecture

Raw CSV Dataset\
↓\
Data Cleaning (Pandas - Jupyter Notebook)\
↓\
MySQL Database (customer table)\
↓\
Advanced SQL Queries\
↓\
Power BI Dashboard (DAX + Visualizations)

------------------------------------------------------------------------

## 🛠️ Tech Stack

-   Python (Pandas, NumPy)
-   MySQL
-   SQLAlchemy & PyMySQL
-   Power BI
-   DAX

------------------------------------------------------------------------

## 🧹 Data Cleaning & Feature Engineering

Notebook: `customer_purchasing_behaviour.ipynb`

Key Steps: - Loaded dataset using Pandas - Checked missing values & data
types - Filled missing review ratings using category-wise median -
Standardized column names (lowercase & snake_case) - Renamed
purchase_amount\_(usd) → purchase_amount - Created age_group using
quartile segmentation - Converted purchase frequency into numeric days -
Validated discount & promo code consistency - Exported cleaned data to
MySQL

------------------------------------------------------------------------

## 🗄️ Database Integration

Stored cleaned dataset in MySQL:

df.to_sql("customer", engine, if_exists="replace", index=False)

Created structured table: `customer`

------------------------------------------------------------------------

## 🔎 SQL Analysis

File: `customer_behaviour_sql_queries.sql`

Business Questions Answered: - Revenue by gender - High-spend customers
using discounts - Top 5 products by average rating - Shipping type
purchase comparison - Subscriber vs non-subscriber revenue - Discount
percentage by product - Customer segmentation (New / Returning /
Loyal) - Top 3 products per category (Window Function) - Repeat buyer
subscription behavior - Revenue contribution by age group

SQL Concepts Used: - GROUP BY & Aggregations - Subqueries - CASE
statements - CTE (WITH clause) - Window Functions (ROW_NUMBER) -
Conditional Aggregation - ORDER BY & LIMIT

------------------------------------------------------------------------

## 📊 Power BI Dashboard

File: `customer_behavior_dashboard.pbix`

Dashboard Pages:

1.  Executive Overview
2.  Customer Segmentation
3.  Product & Category Analysis
4.  Behavioral Insights

------------------------------------------------------------------------

## 🚀 How to Run

1.  Run customer_purchasing_behaviour.ipynb
2.  Push cleaned data to MySQL
3.  Execute customer_behaviour_sql_queries.sql
4.  Open customer_behavior_dashboard.pbix in Power BI


