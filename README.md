# 📊 SQL Data Analytics Project

An end-to-end **SQL Server Data Analytics project** focused on analyzing customer, product, and sales data to uncover business insights and performance trends.

The project demonstrates practical SQL skills used in real-world data analysis, from data exploration and KPI calculation to advanced analytics and reusable reporting views.

---

## 🛠️ Tech Stack

* **Microsoft SQL Server**
* **T-SQL**
* **SQL Server Management Studio (SSMS)**

---

## 📂 Project Structure

```text
sql-data-analytics-project/
│
├── datasets/
│   └── csv_files/
│       ├── bronze/
│       ├── silver/
│       └── gold/
│
├── scripts/
│   ├── 0_init_database.sql
│   ├── 1_database_exploration.sql
│   ├── 2_dimensions_exploration.sql
│   ├── 3_date_range_exploration.sql
│   ├── 4_measures_exploration.sql
│   ├── 5_magnitude_analysis.sql
│   ├── 6_ranking_analysis.sql
│   ├── 7_change_over_time_analysis.sql
│   ├── 8_cumulative_analysis.sql
│   ├── 9_performance_analysis.sql
│   ├── 10_data_segmentation.sql
│   ├── 11_part_to_whole_analysis.sql
│   ├── 12_report_customers.sql
│   └── 13_report_products.sql
│
└── README.md
```

---

## 🔍 Analysis Performed

### 📈 Sales & KPI Analysis

* Total sales, orders, quantity and average selling price
* Sales distribution across customers and product categories
* Category contribution to overall revenue

### 👥 Customer Analysis

* Customer distribution by country and demographics
* Top and bottom customers by revenue
* Customer recency, lifespan and spending analysis
* VIP, Regular and New customer segmentation

### 📦 Product Analysis

* Product and category performance
* Top and bottom performing products
* Product revenue and customer reach
* High, Mid and Low performer segmentation

### 📅 Time-Series Analysis

* Monthly sales trends
* Running totals
* Moving averages
* Year-over-Year performance comparison

---

## 🧠 SQL Skills Demonstrated

```text
✔ Joins
✔ CTEs
✔ Subqueries
✔ Aggregate Functions
✔ CASE Statements
✔ Window Functions
✔ RANK()
✔ LAG()
✔ Running Totals
✔ Time-Series Analysis
✔ Data Segmentation
✔ SQL Views
```

---

## 🏗️ Data Model

The analysis is built around a simple analytical warehouse structure:

```text
             dim_customers
                   │
                   │
                   ▼
              fact_sales
                   ▲
                   │
                   │
              dim_products
```

### Gold Layer

* `gold.dim_customers`
* `gold.dim_products`
* `gold.fact_sales`

Reusable reporting views:

* `gold.report_customers`
* `gold.report_products`

---

## 📊 Reporting Views

### Customer Report

Provides customer-level metrics including:

* Total orders
* Total sales
* Total quantity
* Products purchased
* Customer lifespan
* Recency
* Average Order Value
* Customer segment

### Product Report

Provides product-level metrics including:

* Total orders
* Total sales
* Total quantity
* Total customers
* Average selling price
* Product lifespan
* Recency
* Average monthly revenue
* Product performance segment

These views can also be used as a **data source for Power BI or other BI tools**.

---

## 🚀 How to Run

### 1. Clone the repository

```bash
git clone https://github.com/amittt-k/sql-data-analytics-project.git
```

### 2. Open the project in SQL Server Management Studio

Run the scripts in the following order:

```text
0_init_database.sql
1_database_exploration.sql
2_dimensions_exploration.sql
...
13_report_products.sql
```

> **Note:** Update the `BULK INSERT` file paths in `0_init_database.sql` to match the location of the CSV files on your system.

---

## 🎯 Key Takeaway

This project demonstrates how **SQL can transform raw transactional data into meaningful business insights** through structured analysis, advanced SQL techniques, customer/product segmentation, and reusable reporting datasets.

---

## 👨‍💻 Author

**Amit Kumar**
B.Tech Computer Engineering — IIIT Bhubaneswar

[GitHub](https://github.com/amittt-k)

