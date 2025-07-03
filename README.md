# Task 7: Basic Sales Summary with SQLite in Python

## Overview
This script connects to an SQLite database, runs an SQL query to summarize sales data by product, and visualizes revenue using a bar chart.

## Tools Used
- Python
- SQLite3
- Pandas
- Matplotlib

## Output
- Total quantity and revenue per product printed.
- Revenue chart saved as `sales_chart.png`.

## SQL Query Explained
```sql
SELECT product,
       SUM(quantity) AS total_qty,
       SUM(quantity * price) AS revenue
FROM sales
GROUP BY product;
