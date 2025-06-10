# 📊 advanced-sql-learning

**30-day advanced SQL learning journey** with real-world queries, performance tuning, stored procedures, and project-based practice.  
Built to demonstrate hands-on experience for **Data Analysts**, **Database Developers**, and **DevOps Engineers**.

> 🧑‍💻 Note: This repository skips beginner-level SQL (`SELECT`, `WHERE`, etc.)  
> and directly focuses on real-world intermediate to advanced scenarios  
> used in production environments.

---

## 📅 Daily Learning Schedule

| Day | Topic | Folder |
|-----|--------------------------|-------------------|
| 1 | Advanced Joins | `day-01-joins/` |
| 2 | Subqueries | `day-02-subqueries/` |
| 3 | Group By + HAVING | `day-03-groupby-having/` |
| 4 | Window Functions (Part 1) | `day-04-window1/` |
| 5 | Window Functions (Part 2) | `day-05-window2/` |
| 6 | Common Table Expressions (CTEs) | `day-06-ctes/` |
| 7 | Practice Day (Week 1 Review) | `day-07-practice/` |
| 8 | Index Basics | `day-08-indexes/` |
| 9 | Query Optimization Techniques | `day-09-optimization/` |
|10 | Execution Plans | `day-10-execution-plans/` |
|11 | Transactions (BEGIN, COMMIT, ROLLBACK) | `day-11-transactions/` |
|12 | Isolation Levels & Locking | `day-12-isolation-levels/` |
|13 | Deadlocks & Solutions | `day-13-deadlocks/` |
|14 | Practice Day (Week 2 Review) | `day-14-practice/` |
|15 | Self Join, Cross Apply | `day-15-advanced-joins/` |
|16 | PIVOT / UNPIVOT | `day-16-pivot-unpivot/` |
|17 | Working with JSON | `day-17-json/` |
|18 | Working with XML | `day-18-xml/` |
|19 | CASE WHEN Logic | `day-19-case-when/` |
|20 | Filtered Aggregations | `day-20-aggregations/` |
|21 | Mini Project: Analytics Report | `day-21-mini-project/` |
|22 | Stored Procedures | `day-22-stored-procedures/` |
|23 | Scalar & Table-Valued Functions | `day-23-functions/` |
|24 | Error Handling in SQL | `day-24-error-handling/` |
|25 | Triggers | `day-25-triggers/` |
|26 | Dynamic SQL | `day-26-dynamic-sql/` |
|27 | Role-Based Access & Permissions | `day-27-permissions/` |
|28 | Practice Day (Week 4 Review) | `day-28-practice/` |
|29 | Capstone Project | `capstone-project/` |
|30 | Final README Polish & Docs | `README.md` |

---

## 🧠 What You'll Find Here

- 🛠 **Real-world SQL scenarios**
- 🪄 **Performance-tuned queries**
- 📈 **Window functions & CTEs**
- 🧮 **Stored procedures and functions**
- 🔐 **Transactions, Triggers, Indexes**
- 🚀 **Capstone project with analytics queries**

---

## 🧪 Sample Code Snippet

```sql
-- Calculate running total of sales per employee
SELECT 
  employee_id,
  sale_amount,
  SUM(sale_amount) OVER (PARTITION BY employee_id ORDER BY sale_date) AS running_total
FROM sales_data;
