# -Pizza-Sales
Business Analyst Internship Projects at Unified Mentor (SQL, Power BI, Excel)
🍕 Pizza Sales Dashboard (Power BI + SQL)
📌 Project Overview
This project was developed as part of my Business Analyst Internship at Unified Mentor.
The goal was to analyze pizza sales data (2015) using SQL and Power BI to generate actionable insights.
SQL was used for data cleaning, joins, aggregations, and KPIs.
Power BI was used for dashboard design, DAX measures, and visualization.

🗄 SQL Work

Key SQL tasks performed:
✅ Cleaned and structured raw sales dataset
✅ Used joins to merge order, pizza, and category data
✅ Wrote aggregate queries (SUM, COUNT, AVG) for KPIs like Revenue, Total Orders, Avg Order Value
✅ Created CTEs & Window Functions for trend analysis (hourly/weekly sales)
✅ Exported clean dataset to Power BI for visualization

📌 Example SQL Queries:

-- Total Revenue
SELECT SUM(total_price) AS Total_Revenue
FROM pizza_sales;

-- Average Order Value
SELECT SUM(total_price) / COUNT(DISTINCT order_id) AS Avg_Order_Value
FROM pizza_sales;

-- Total Pizzas Sold
SELECT SUM(quantity) AS Total_Pizzas
FROM pizza_sales;

-- Hourly Sales Trend
SELECT DATEPART(HOUR, order_time) AS OrderHour, COUNT(order_id) AS TotalOrders
FROM pizza_sales
GROUP BY DATEPART(HOUR, order_time)
ORDER BY OrderHour;

📊 Dashboard Pages
Page 1: Sales Overview

KPIs (Orders, Pizzas Sold, Revenue, AOV, Avg Pizzas/Order)
Hourly & Weekly Sales Trends
Category & Size Performance

Page 2: Best & Worst Sellers

Top 5 & Bottom 5 pizzas by Revenue, Quantity, and Orders
Helps business identify popular pizzas and underperforming items

🔑 Key Insights

📈 Total Orders: 21K
🍕 Total Pizzas Sold: 50K
💰 Total Revenue: $817.86K
🕒 Busiest Hour: 12 PM
📅 Busiest Week: Week 48
🍕 Best Category: Classic Pizzas
📉 Worst Performing Size: XXL

🛠 Tools & Skills Used

SQL (Data Cleaning, Joins, Aggregates, Window Functions)
Power BI (Data Modeling, DAX, Visualization)
Excel/CSV (Preprocessing)
Business Analysis Skills: KPI design, Sales trend analysis, Best/Worst performer analysis

📸 Dashboard Preview


## 👩‍💻 About Me
Created by **Sapna** – Business Analyst Intern @ Unified Mentor  

📧 Email: businessanalystsapna@gmail.com  
🌐 GitHub: [Sapnaba07](https://github.com/Sapnaba07)  
💼 LinkedIn: [www.linkedin.com/in/sapna-patel-587b40375  
