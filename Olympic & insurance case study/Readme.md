# Olympic & Insurance Case Study

## Introduction
This repository contains SQL case studies focusing on **Olympic Games** and **Insurance Data** analysis. The project demonstrates how to extract insights from structured data using SQL queries, covering various analytical aspects such as aggregation, filtering, ranking, and complex joins.

## Datasets
1. **Olympic Dataset**
   - Contains details of athletes, countries, events, and results.
   - Used to analyze trends, medal counts, and athlete performances.
2. **Insurance Dataset**
   - Includes information about policyholders, claims, and premiums.
   - Used for risk assessment, fraud detection, and customer segmentation.

## Objectives
- To gain insights into Olympic performances over the years.
- To understand customer trends and risk factors in the insurance industry.
- To apply SQL techniques for data extraction and decision-making.

## SQL Techniques Used
- **Filtering and Aggregation** (`WHERE`, `GROUP BY`, `HAVING`, `COUNT`, `SUM`, `AVG`)
- **Sorting and Ranking** (`ORDER BY`, `RANK()`, `DENSE_RANK()`)
- **Joins and Subqueries** (`INNER JOIN`, `LEFT JOIN`, `RIGHT JOIN`, `SUBQUERY`)
- **Window Functions** (`ROW_NUMBER()`, `PARTITION BY`)
- **Case Statements** (`CASE WHEN` for conditional logic)

## Example Queries
### 1. Top 10 Countries by Total Olympic Medals
```sql
SELECT country, SUM(gold + silver + bronze) AS total_medals
FROM olympic_medal_table
GROUP BY country
ORDER BY total_medals DESC
LIMIT 10;
```

### 2. Insurance Claim Count by Customer Category
```sql
SELECT customer_category, COUNT(claim_id) AS total_claims
FROM insurance_claims
GROUP BY customer_category;
```

## How to Use
1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/olympic-insurance-case-study.git
   ```
2. Import the SQL file into your database.
3. Run the queries using a SQL client like MySQL Workbench, PostgreSQL, or any preferred tool.

## Conclusion
This case study provides a hands-on approach to analyzing real-world datasets using SQL. It helps in understanding historical trends in the Olympics and risk factors in insurance industries.

## Author
[Bhoopendra Vishwakarma](https://github.com/yourusername)

