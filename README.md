# 📚 Online Bookstore Sales Analysis using PostgreSQL

> An end-to-end SQL Data Analytics project demonstrating database design, data import, SQL querying, and business insight generation using PostgreSQL.

![SQL](https://img.shields.io/badge/SQL-PostgreSQL-blue?style=for-the-badge)
![Level](https://img.shields.io/badge/Level-Beginner-success?style=for-the-badge)
![Database](https://img.shields.io/badge/Database-PostgreSQL-336791?style=for-the-badge)

---

# 📌 Project Overview

This project simulates an **Online Bookstore Management System** where books, customers, and orders are stored in a relational database.

The project focuses on designing a relational database, importing CSV datasets, writing SQL queries, and extracting meaningful business insights from transactional data.

It is designed to strengthen SQL skills commonly required for **Data Analyst** and **Business Analyst** roles.

---

# 🎯 Business Objectives

- Design a relational database
- Import CSV datasets into PostgreSQL
- Analyze customer purchasing behavior
- Evaluate book sales performance
- Monitor inventory levels
- Generate revenue insights
- Practice interview-oriented SQL queries

---

# 🛠 Tech Stack

- **Database:** PostgreSQL
- **Language:** SQL
- **Dataset:** CSV Files
- **IDE:** pgAdmin 4

---

# 📂 Project Structure

```
Online-Bookstore-SQL-Project/

│── Dataset/
│   ├── Books.csv
│   ├── Customers.csv
│   └── Orders.csv
│
│── OnlineBookstore.sql
│
├── README.md
```

---

# 🗄 Database Schema

The project contains three relational tables.

## 📖 Books

| Column | Description |
|---------|-------------|
| Book_ID | Primary Key |
| Title | Book Name |
| Author | Author Name |
| Genre | Category |
| Published_Year | Publication Year |
| Price | Book Price |
| Stock | Available Stock |

---

## 👤 Customers

| Column | Description |
|---------|-------------|
| Customer_ID | Primary Key |
| Name | Customer Name |
| Email | Email Address |
| Phone | Contact Number |
| City | City |
| Country | Country |

---

## 🛒 Orders

| Column | Description |
|---------|-------------|
| Order_ID | Primary Key |
| Customer_ID | Foreign Key |
| Book_ID | Foreign Key |
| Order_Date | Purchase Date |
| Quantity | Books Purchased |
| Total_Amount | Order Value |

---

# 🔗 Database Relationships

```
Customers
    │
    ▼
 Orders
    ▲
    │
Books
```

- One Customer → Many Orders
- One Book → Many Orders
- Orders table connects Customers and Books

---

# 📥 Data Import

The datasets were imported into PostgreSQL using the **COPY** command.

- Books.csv
- Customers.csv
- Orders.csv

---

# 📊 SQL Analysis Performed

## Basic SQL Queries

✔ Retrieve books by genre

✔ Find books published after a specific year

✔ Retrieve customers by country

✔ Filter orders by date

✔ Calculate total inventory

✔ Find the most expensive book

✔ Find books with lowest stock

✔ Calculate total revenue

✔ Retrieve distinct genres

✔ Filter orders by quantity and amount

---

## Business Analysis Queries

### 📚 Total Books Sold by Genre

Used **JOIN**, **SUM()**, and **GROUP BY** to determine best-selling genres.

---

### 💰 Average Price of Fantasy Books

Calculated average book price using **AVG()**.

---

### 👥 Repeat Customers

Identified customers who placed multiple orders using **GROUP BY** and **HAVING**.

---

### 🔥 Most Frequently Ordered Book

Ranked books based on customer demand using **COUNT()**.

---

### 📖 Top 3 Most Expensive Fantasy Books

Filtered books by genre and ranked using **ORDER BY**.

---

### ✍️ Author Sales Performance

Calculated total quantity sold for each author.

---

### 🌍 Customer Cities with High Spending

Identified cities where customers spent more than \$30.

---

### 💵 Highest Spending Customer

Calculated total customer spending using **SUM()**.

---

### 📦 Remaining Inventory

Calculated remaining stock after fulfilling customer orders using:

- LEFT JOIN
- COALESCE()
- Aggregate Functions

---

# 📈 Business Insights

- Fiction and Fantasy genres generate strong sales.
- A small number of books contribute significantly to total revenue.
- Repeat customers increase overall business value.
- Inventory analysis helps identify books that require restocking.
- Customer spending patterns highlight high-value customers.
- Sales reports support pricing and inventory decisions.

---

# 🧠 SQL Concepts Demonstrated

- Database Design
- Primary Keys
- Foreign Keys
- INNER JOIN
- LEFT JOIN
- GROUP BY
- HAVING
- ORDER BY
- Aggregate Functions
- Filtering
- DISTINCT
- Date Filtering
- COALESCE()
- Inventory Calculations
- Business Reporting

---

# 🚀 How to Run This Project

### 1️⃣ Create Database

```sql
CREATE DATABASE OnlineBookstore;
```

### 2️⃣ Connect Database

```sql
\c OnlineBookstore
```

### 3️⃣ Execute SQL File

Run:

```
OnlineBookstore.sql
```

This script will:

- Create all tables
- Import CSV data
- Execute all SQL queries
- Generate business reports

---

# 🎯 Learning Outcomes

Through this project I strengthened my understanding of:

- Relational Database Design
- PostgreSQL
- SQL Query Writing
- SQL Aggregations
- SQL Joins
- Business-Oriented Data Analysis
- Inventory Analysis
- Reporting & Decision Making

---

# 📸 Project Preview

Add screenshots for:

- Database Tables
- PostgreSQL Output
- SQL Query Results
- Execution Screenshots
- ER Diagram (Optional)

---

# ⭐ Key Features

- Beginner-Friendly
- End-to-End SQL Project
- Real Business Scenario
- Interview-Oriented Queries
- Well Structured SQL Script
- Clean Database Design
- Business Insights

---

# 👨‍💻 Author

**Sanjay Chourasiya**

**Aspiring Data Analyst**

### Skills

- PostgreSQL
- SQL
- Excel
- Power BI
- Python

---

⭐ **If you found this project helpful, consider giving it a Star on GitHub!**
