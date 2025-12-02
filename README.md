# 🛒 E-Commerce Order Analysis using SQL

This project is a complete SQL-based analysis of an **E-Commerce Order Dataset**.  
It showcases end-to-end skills used by Data Analysts, including data modeling, table creation, data insertion, joins, aggregations, window functions, and business insights.

This is **Project #1** in my SQL portfolio.

---

## 🎯 Project Objectives

- Design an e-commerce database from scratch  
- Create tables for customers, products, orders & order_items  
- Insert sample realistic transactional data  
- Perform SQL analysis to answer business questions:  
  - Total revenue  
  - Monthly/weekly sales trends  
  - Top-selling products  
  - Best customers  
  - Category performance  
  - Order size analysis  
  - Repeat customers  
- Use joins, CTEs, subqueries, window functions  

---

## 🛠️ Tools & Technologies

- **SQL (MySQL / PostgreSQL / SQL Server)**  
- Any SQL client (DBeaver, MySQL Workbench, pgAdmin)  
- GitHub for version control  

---

## 🗂️ Database Schema

### **1. customers**
| field | type | description |
|-------|--------|-------------|
| customer_id | INT (PK) | Unique customer |
| customer_name | VARCHAR | Customer name |
| email | VARCHAR | Email address |
| city | VARCHAR | Customer location |
| state | VARCHAR | State |
| created_at | DATE | Customer registration date |

---

### **2. products**
| field | type | description |
|-------|--------|-------------|
| product_id | INT (PK) | Unique product |
| product_name | VARCHAR | Name |
| category | VARCHAR | Electronics / Fashion / Home etc |
| price | DECIMAL | Unit price |

---

### **3. orders**
| field | type | description |
|-------|--------|-------------|
| order_id | INT (PK) | Unique order |
| customer_id | INT (FK) | Linked to customers |
| order_date | DATE | When order placed |
| status | VARCHAR | Delivered / Cancelled / Returned |

---

### **4. order_items**
| field | type | description |
|-------|--------|-------------|
| item_id | INT (PK) | Unique item line |
| order_id | INT (FK) | Which order |
| product_id | INT (FK) | Product purchased |
| quantity | INT | Units |
| unit_price | DECIMAL | Price at purchase time |

---

## 🧪 Analysis Performed

All queries are available in `analysis_queries.sql`.

### Key Metrics:
- 📌 Total Revenue  
- 📌 Total Orders  
- 📌 Average Order Value (AOV)  
- 📌 Revenue by Product Category  
- 📌 Best Selling Products  
- 📌 Top 10 Customers by Revenue  
- 📌 Monthly Revenue Trend  
- 📌 Repeat Customer Rate  
- 📌 Cancelled / Returned Orders Analysis  
- 📌 Order size distribution  

---
