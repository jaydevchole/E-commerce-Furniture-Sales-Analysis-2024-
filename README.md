# E-commerce-Furniture-Sales-Analysis-2024
This is my first Git Repository.
/ecommerce-sql-analysis
│
├── 📂 SQL
│   ├── create_tables.sql
│   ├── insert_data.sql
│   ├── analysis_queries.sql
│   └── views_and_ctes.sql
│
├── 📜 README.md
├── 📄 ERD.png  (optional - Entity Relationship Diagram)
├── 📁 Data (optional)
│   └── ecommerce_data_sample.csv
└── 📁 Screenshots (optional - if using a BI tool too)



CREATE TABLE Customers (
    CustomerID INT PRIMARY KEY,
    CustomerName VARCHAR(100),
    Segment VARCHAR(50)
);



-- Top 5 best-selling products
SELECT ProductName, SUM(Sales) AS TotalSales
FROM Orders
GROUP BY ProductName
ORDER BY TotalSales DESC
LIMIT 5;






# Initialize Git
git init

# Add files
git add .

# Commit changes
git commit -m "Initial commit - added SQL scripts"

# Connect to GitHub repo
git remote add origin https://github.com/yourusername/ecommerce-sql-analysis.git

# Push to GitHub
git push -u origin main







# 🗃️ E-commerce Sales Analysis (SQL)

**Tools:** SQL (PostgreSQL / MySQL / SQL Server), Git  
**Role:** Data Analyst / SQL Developer  
**Duration:** Sept 2025

---

## 📌 Overview
This project explores and analyzes sales data from a fictional e-commerce company using SQL queries. The goal is to extract business insights on customer segments, regional performance, and product sales.

---

## 🔧 SQL Topics Covered
- Table creation and schema design
- Data cleaning with SQL
- CTEs and subqueries
- Window functions
- Aggregate analysis (SUM, AVG, COUNT)
- Joins and filtering

---

## 🔍 Sample Insights
- Top 5 best-selling products by revenue
- Monthly sales trends by region
- Profitability by customer segment
- Average order value per region

---

## 📁 Files
- `create_tables.sql` – SQL schema for tables
- `insert_data.sql` – Sample data inserts
- `analysis_queries.sql` – Business logic queries
- `views_and_ctes.sql` – Optimized reporting queries using CTEs

---

## 🚀 Getting Started
1. Clone the repo:
   ```bash
   git clone https://github.com/yourusername/ecommerce-sql-analysis.git



