# Sales-Summary-from-a-Tiny-SQLite-Database-using-Python
🔍 Project Title
Task 7: Basic Sales Summary from a Tiny SQLite Database using Python

🎯 Objective
This task demonstrates how to connect a Python script to an SQLite database, perform SQL queries to summarize sales data, and visualize the results with a simple bar chart.

🧰 Tools & Technologies Used
Python

SQLite (sqlite3 module)

Pandas

Matplotlib

Google Colab

📁 Files Included
File Name	Description
Task_7.ipynb	Main notebook containing code, SQL execution, and chart
Screenshot_125416.png	Output screenshot of the printed sales summary table
Screenshot_125524.png	Output screenshot of the bar chart (Revenue by Product)
README.md	This file — task description and summary

🧮 Overview
A sales table was created with product data.

SQL was used to group data and compute:

Total quantity sold per product

Total revenue (quantity × price)

Results were imported into a pandas DataFrame and printed.

A bar chart was generated to visualize total revenue per product.

🧾 SQL Query Used
sql
Copy
Edit
SELECT 
    product,
    SUM(quantity) AS total_qty,
    SUM(quantity * price) AS revenue
FROM sales
GROUP BY product;
🖼️ Sample Output
Sales Summary Table
(Product-wise quantity and revenue):

Product	Total Quantity	Revenue ($)
Apple	75	37.5
Banana	75	22.5
Orange	60	42.0

Bar Chart:
A bar chart visualizing the revenue of each product clearly shows that:

Orange has the highest revenue.

Followed by Apple.

Banana has the lowest revenue.

