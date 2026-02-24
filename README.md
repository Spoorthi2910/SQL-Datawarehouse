# SQL-Datawarehouse
Project Overview

This project focuses on building a structured SQL-based Data Warehouse from raw business data to generate meaningful insights. The goal was to design a clean, scalable data model and create business-ready reports that help in analyzing customer behavior, product performance, and overall sales trends.Instead of just writing queries, this project demonstrates how raw transactional data can be transformed into analytical datasets using proper schema design, data modeling, and reporting logic.

Tech Stack
SQL (Data cleaning, transformation, reporting logic)
Data Warehouse concepts (Fact & Dimension modeling)
Star Schema design
Views for reporting layer

Project Architecture
The project is structured into three main layers:
1. Raw Layer
Contains raw source tables such as:
Customer information
Product details
Sales transactions
This layer represents the original, unprocessed data.

2. Gold Layer (Reporting Layer)
This layer contains transformed and analytics-ready views created using SQL.
Example:
report_customers
report_products
These views combine multiple tables, apply transformations, and calculate business metrics.
Data Modeling Approach
I used a Star Schema model:
Fact Table:
Sales (contains transactional data such as order date, order number, revenue, cost, etc.)
Dimension Tables:
Customers (customer details and segmentation)
Products (product category, subcategory, cost)

This structure improves query performance and makes reporting easier.

Key Reports Created
1. Customer Report
Purpose:
To analyze customer-level performance and behavior.
Includes:
Customer details
Total orders
Total revenue
Total quantity purchased
Profit
Customer segmentation insights
Why I built this:
To understand high-value customers, repeat buyers, and customer contribution to revenue.
2. Product Report
Purpose:
To analyze product performance across categories and subcategories.
Includes:
Product name
Category and subcategory
Total sales
Total quantity sold
Total cost
Profit
Order trends
Why I built this:
To identify best-performing products, loss-making products, and category-level trends.

Business Insights Generated
Identified top revenue-generating customers
Analyzed product categories contributing most to profit
Evaluated sales trends over time
Compared revenue vs cost to calculate profitability

Created a structured reporting system for business monitoring
