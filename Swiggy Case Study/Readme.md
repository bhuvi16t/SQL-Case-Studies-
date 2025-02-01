# SQL Swiggy Case Study 🍽️

## 📌 Overview
This repository contains an **SQL case study on Swiggy**, focusing on analyzing restaurant data, customer orders, and delivery trends. The dataset and queries help extract meaningful insights into food delivery patterns, customer behavior, and business performance.

## 📂 Files
- **SQL-Swiggy-Case-Study.sql** – SQL queries for data analysis, including:
  - Data cleaning & preprocessing
  - Customer order insights
  - Revenue and sales trends
  - Delivery performance analysis

## 🛠️ Technologies Used
- **SQL** (MySQL / PostgreSQL)
- **Database Management**
- **Data Analysis Techniques**

## 🚀 Key Analysis Areas
1. **Order Trends** – Analyzing peak order times and most popular cuisines.
2. **Customer Behavior** – Identifying loyal customers and order frequency.
3. **Revenue Insights** – Finding top-grossing restaurants and average order values.
4. **Delivery Performance** – Evaluating delivery speed and efficiency.

## 📊 Sample Queries
```sql
-- Retrieve top 5 restaurants with the highest total revenue
SELECT restaurant_name, SUM(total_price) AS total_revenue
FROM orders
GROUP BY restaurant_name
ORDER BY total_revenue DESC
LIMIT 5;
