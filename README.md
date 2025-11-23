# Northwind Traders Analytics (SQL with Jupysql)

## Overview
This project demonstrates SQL analysis on the Northwind trading company dataset. It covers schema exploration, sales KPIs, geographic revenue, product and supplier performance, monthly trends, employee sales, customer segmentation, and Pareto checks. Each query is explained clearly and runnable in a SQL-only Jupyter notebook using Jupysql.

## Dataset
- SQLite database: `data/northwind.db`
- Key tables: Orders, "Order Details", Customers, Products, Suppliers, Employees
- Relationships:
  - Orders → Customers
  - Orders → Employees
  - "Order Details" → Products → Suppliers

## How to run
1. Ensure `northwind.db` is present.
2. Open `northwind_traders_analytics_sql.ipynb`.
3. Run the setup cells:
   ```python
   %load_ext sql
   %sql sqlite:///northwind.db
4. Execute sections in order. Each has a short explanation and a %%sql query.

## Query index
- Setup & schema: list tables, PRAGMA structures
- KPIs: total sales, orders, customers, average order value
- Geography: revenue by country
- Products: top products by sales
- Suppliers: supplier revenue
- Time: monthly sales trend
- Employees: sales performance
- Customers: lifetime value and order counts
- Pareto: top 20% customers’ revenue share

## Highlights
- 12 Tables Queried
- 7 Complex Joins
- 25+ Business KPIs Extracted

## Technologies
- SQL
- SQLite
- Jupyter Notebook
- Jupysql

## Notes
- Strictly SQL cells using Jupysql.
- Portable paths; no personal directories.
- "Order Details" table name includes a space and must be quoted in queries.
