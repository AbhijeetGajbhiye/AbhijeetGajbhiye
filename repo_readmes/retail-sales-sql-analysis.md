# 🛒 Retail Sales Analysis — SQL

> Answer business questions directly from a normalized retail database using SQL.

### The project

A SQL-first analysis of a **4-table retail database** covering roughly **1,700 orders and 500 customers over 15 months**.

The focus isn't on showing off syntax — it's on using SQL to answer questions a business could actually act on.

### Questions answered

**01 — Revenue trend**  
Monthly revenue and average order value to understand the growth trajectory.

**02 — Product concentration**  
The top five products account for about **40% of total revenue** despite representing only five of twenty SKUs.

**03 — Stockout risk**  
A rolling 60-day sales window is used to estimate "days of cover" and identify products that need attention.

**04 — Cohort retention**  
Month-by-month retention by signup cohort using CTEs and date arithmetic.

**05 — Regional top spenders**  
Window functions identify the top three customers in each region.

### SQL techniques

`JOIN` · `GROUP BY` · `CTE` · `RANK()` · window functions · date arithmetic · derived metrics

### Stack

`SQL` `SQLite` `Python`

### Files

- `retail.db` — database
- `analysis_queries.sql` — commented analysis queries
- `generate_sql_data.py` — dataset generator
- `chart*.png` — output charts
