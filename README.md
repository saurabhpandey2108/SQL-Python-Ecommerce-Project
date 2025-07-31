# 🛒 SQL + Python E-Commerce Analysis Project

An end-to-end exploratory data analysis (EDA) and insights generation project for an e-commerce platform using **SQL** and **Python**. This project covers data cleaning, advanced SQL querying, and Python-based visualization to help businesses derive actionable insights from customer transactions and behavior.

## 📌 Project Objectives

- Analyze customer, order, product, and payment data from an e-commerce platform.
- Perform data cleaning and transformation using SQL and Python (Pandas).
- Identify key performance metrics such as top-selling products, high-value customers, repeat buyers, etc.
- Generate clear, compelling visualizations for stakeholder reporting.

---

## 🧰 Tools & Technologies Used

| Tool | Purpose |
|------|---------|
| **MySQL / SQL** | Data extraction, transformation, complex querying |
| **Python (Pandas, Matplotlib, Seaborn)** | Data manipulation and visualization |
| **Jupyter Notebook** | Analysis workflow and documentation |
| **Excel** | Preliminary exploration and cross-verification (optional) |

---

## 📂 Project Structure

SQL-Python-Ecommerce-Project/
│
├── SQL/
│ ├── create_tables.sql # Schema definition
│ ├── data_queries.sql # Key business queries
│ └── insights_queries.sql # Analytical SQL queries
│
├── Python/
│ ├── ecommerce_analysis.ipynb # Python EDA and visualization
│ └── plots/ # Saved plots/images
│
├── Data/
│ └── ecommerce_dataset.csv # E-commerce transactional dataset
│
└── README.md # Project overview

---

## 📊 Key Insights

- Identified top 10 best-selling products by quantity and revenue.
- Analyzed monthly trends in revenue and order volume.
- Segmented customers based on purchase behavior (one-time vs repeat buyers).
- Highlighted products with high return rates or low conversion.
- Visualized category-wise and location-wise customer preferences.

---

## 🔍 Sample SQL Queries

```sql
-- Top 5 customers by total purchase amount
SELECT customer_id, SUM(total_amount) AS total_spent
FROM orders
GROUP BY customer_id
ORDER BY total_spent DESC
LIMIT 5;
