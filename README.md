# 📊 SQL Case Studies Repository

## 📌 Overview
This repository contains multiple SQL case studies analyzing different real-world datasets, including **Olympics, Insurance, Swiggy, Pizza Sales, and Smartphone Market Trends**. Each case study includes SQL queries for **data cleaning, analysis, and insights**.

## 📂 Case Studies Included
1. **🏅 Olympic Case Study** – Analyzing athlete performance, country rankings, and medal trends.
2. **📄 Insurance Case Study** – Investigating claim patterns, customer demographics, and risk analysis.
3. **🍽️ Swiggy Case Study** – Examining food delivery trends, restaurant sales, and customer behavior.
4. **🍕 Pizza Sales Analysis** – Understanding sales trends, top-selling pizzas, and revenue insights.
5. **📱 Smartphone Market Study** – Exploring brand performance, sales distribution, and market trends.

## 🛠️ Technologies Used
- **SQL (MySQL / PostgreSQL)**
- **Database Management**
- **Data Cleaning & Transformation**
- **Business Insights & Analytics**

## 📊 Sample Query
```sql
-- Find the top 5 countries with the most Olympic gold medals
SELECT country, COUNT(*) AS gold_medals
FROM olympics_data
WHERE medal = 'Gold'
GROUP BY country
ORDER BY gold_medals DESC
LIMIT 5;
