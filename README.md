# Product Performance Analysis - Identifying Best and Worst-Selling Products with Seasonal Trends

## Objective: 
To analyse product sales by looking at the best and worst-performing products, tracking seasonal trends, and identifying fluctuations in sales.

---
## Tables/Columns Used:
products 
(columns: product_id, product_name)

sales 
(columns: sale_id, product_id, amount, quantity_sold, sale_date)

---
## Explanation:

The product_sales CTE aggregates product sales by month and year, including total revenue, units sold, and transactions.

The seasonal_sales CTE calculates the average sale price and ranks products based on total revenue within each year.

Window Function: PERCENT_RANK() is used to rank products by total revenue within each year.

The query also classifies sales data into seasonal categories (e.g., Holiday, Summer, Off-Peak) based on the month of sale.
