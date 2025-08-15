# Elevate_Labs_Task7

# Task 7 - Basic Sales Summary using SQLite and Python in Google Colab

##  Overview
This project demonstrates how to connect Python to a small SQLite database, run basic SQL queries, and visualize sales data using Matplotlib — all inside Google Colab.

## Files
- `Task7_Sales_Summary.ipynb` — Colab notebook containing:
  - Database creation with sample sales data.
  - SQL query execution.
  - Data visualization (bar chart).
- `sales_data.db` — SQLite database generated during execution.

## 🛠 Tools Used
- **Python** — for database operations and visualization.
- **SQLite** — lightweight relational database (built into Python).
- **Pandas** — to load SQL query results into a DataFrame.
- **Matplotlib** — for plotting charts.
- **Google Colab** — cloud-based environment to run Python code.

## 📊 SQL Query Explanation
```sql
SELECT 
    product, 
    SUM(quantity) AS total_qty, 
    SUM(quantity * price) AS revenue
FROM sales
GROUP BY product;
