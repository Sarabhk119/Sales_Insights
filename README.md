# Sales Report Dashboard - Alfa Hardware
Dashboard Overview

This Power BI dashboard provides insights into the sales performance of Alfa Hardware. It helps in understanding revenue distribution, sales trends, customer segmentation, and product performance. The dashboard is designed to aid business stakeholders in making data-driven decisions.

Data Source

The raw data was sourced from a MySQL database dump file.

The database was imported into MySQL Server, and necessary transformations were performed using SQL queries before loading it into Power BI.

The dataset contains information related to sales transactions, customers, markets, and products.

Data Extraction & Transformation Steps

Step 1: Import Data into MySQL

The MySQL dump file was restored using the following command:

mysql -u root -p alfa_hardware_db < db_dump.sql;

The relevant tables were analyzed to understand the data structure.

Step 2: Data Cleaning and Preprocessing

Handled missing values: Null values in product names were replaced with "Unknown".

Formatted date columns: Converted transaction dates into YYYY-MM-DD format.

Created new calculated columns: Derived Revenue as Sales Quantity * Unit Price.

Step 3: Data Import into Power BI

A MySQL Connector was used in Power BI to establish a connection with the MySQL database.

The necessary tables were imported, and relationships were established between them.

Dashboard Features

Revenue Metrics: Displays total revenue (142.22M) and total sales quantity (350K).

Revenue by Market: Shows revenue distribution across different markets.

Sales Quantity by Market: Visualizes sales quantity across various market segments.

Revenue Trend Analysis: A line chart depicting monthly revenue trends for the year 2020.

Top 5 Customers: Highlights the highest revenue-generating customers.

Top 5 Products: Displays the best-selling products by revenue.

Time Filters: Allows users to filter data by year and month.

Key Insights

Revenue & Sales Performance
Total Revenue: $142.22M

Total Sales Quantity: 350K

Revenue peaked in early 2020 but showed a declining trend after March 2020.

Market Analysis
Electrical Market contributes the highest revenue (66M), significantly outperforming others.

Excel Stores and Premium Stores are among the top-performing markets.

Customer Insights
Top Customer: Electricalsara Stores (66M in revenue).

The top 5 customers contribute a significant portion of overall revenue.

Product Performance
One of the highest-selling product categories has missing product names, possibly due to data entry issues.

Prod047 and Prod061 are among the best-selling products, but they contribute significantly less than the unknown category.

Business Recommendations

Investigate missing product data to ensure accurate insights into sales performance.

Analyze declining revenue trends post-March 2020 to identify external market factors or operational inefficiencies.

Focus on the electrical market and key customers like Electricalsara Stores for business expansion.

Optimize inventory for top-selling products to ensure demand fulfillment.

Improve data quality in MySQL database by enforcing constraints on missing values.

# Snapshot of powerbi desktop
![Image](https://github.com/user-attachments/assets/d26b2420-5722-4a69-95a6-23dfb9122d6e)

