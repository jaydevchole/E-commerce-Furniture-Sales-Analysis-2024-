# 🛒 E-commerce Furniture Sales Analysis (2024)

> Beginner-friendly SQL project analyzing sales data from a fictional e-commerce furniture company using **SQL Server Management Studio (SSMS)**.

---

## 📌 Project Overview

This project explores **customer segments, product performance, and regional sales trends** from an e-commerce furniture dataset. Using SQL, I extracted insights to support business decision-making.

---

## 🧰 Tools & Technologies

* **SQL Server Management Studio (SSMS)**
* **Git & GitHub** (version control, project sharing)
* *(Optional)* Excel / Power BI / Tableau for visualization

---

## 🧠 SQL Skills Practiced

* Database design (tables, schema creation)
* Data cleaning & insertion
* Querying with `SELECT`, `JOIN`, `WHERE`, `GROUP BY`, `ORDER BY`
* Aggregate functions (`SUM`, `COUNT`, `AVG`, `MAX`, `MIN`)
* CTEs & Views for reusability

---

## 🔍 Business Insights Generated

* 📈 **Top 5 Products** by total revenue
* 🌍 **Monthly Sales Trends** across regions
* 👥 **Customer Segments** driving highest profitability
* 💵 **Average Order Value (AOV)** comparison across regions

---

## 📂 Project Structure

```bash
ecommerce-sql-analysis/
│── create_tables.sql        # Schema creation  
│── insert_data.sql          # Sample dataset insertion  
│── analysis_queries.sql     # Business analysis queries  
│── views_and_ctes.sql       # Predefined views & CTEs for insights  
│── README.md                # Project documentation  
```

---

## 🧑‍💻 Sample Queries

### 1️⃣ Top 5 Products by Revenue

```sql
SELECT TOP 5 
    p.product_name, 
    SUM(o.sales_amount) AS total_revenue
FROM Orders o
JOIN Products p ON o.product_id = p.product_id
GROUP BY p.product_name
ORDER BY total_revenue DESC;
```

### 2️⃣ Average Order Value by Region

```sql
SELECT 
    r.region_name,
    ROUND(SUM(o.sales_amount) * 1.0 / COUNT(DISTINCT o.order_id), 2) AS avg_order_value
FROM Orders o
JOIN Regions r ON o.region_id = r.region_id
GROUP BY r.region_name
ORDER BY avg_order_value DESC;
```

---

## 🚀 How to Run the Project

1. Clone the repo:

   ```bash
   git clone https://github.com/jaydevchole/ecommerce-sql-analysis.git
   cd ecommerce-sql-analysis
   ```
2. Run the SQL scripts in order:

   ```bash
   1. create_tables.sql  
   2. insert_data.sql  
   3. analysis_queries.sql  
   4. views_and_ctes.sql  
   ```

---

## 📌 What I Learned

* Structuring & designing relational databases
* Writing queries to extract actionable business insights
* Using aggregate functions & grouping effectively
* Organizing and documenting a project for GitHub

---

## ✅ Conclusion

This beginner SQL project gave me **hands-on practice** with database design and querying while simulating real-world e-commerce sales analysis.
It improved my ability to connect **technical SQL skills with business problem-solving**.

---

## 📬 Contact

* **LinkedIn:** [Jaydev Chole](https://www.linkedin.com/in/jaydev-chole-b3313b327)
* **Email:** [jaychole2002@gmail.com](mailto:jaychole2002@gmail.com)

---

