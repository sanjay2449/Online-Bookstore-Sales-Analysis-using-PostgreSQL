# 📚 Online Bookstore Sales Analysis using PostgreSQL

> **An end-to-end SQL Data Analytics Project** that demonstrates relational database design, data import, SQL querying, and business insight generation using PostgreSQL.

---

## 📌 Project Overview

This project simulates a real-world **Online Bookstore Management System** where customer purchases, book inventory, and sales transactions are stored in a relational database.

The objective of this project is to transform raw transactional data into meaningful business insights by writing efficient SQL queries and applying database concepts commonly used in data analytics roles.

---

## 🎯 Business Objectives

* Design a normalized relational database
* Import CSV datasets into PostgreSQL
* Analyze customer purchasing behavior
* Evaluate book sales performance
* Monitor inventory levels
* Generate revenue and sales insights
* Practice SQL queries frequently asked in Data Analyst interviews

---

## 🛠 Tech Stack

* **Database:** PostgreSQL
* **Language:** SQL
* **Data Source:** CSV Files
* **IDE:** pgAdmin / PostgreSQL

---

# 📂 Project Structure

```
Online-Bookstore-SQL-Project/

│── Dataset/
│   ├── Books.csv
│   ├── Customers.csv
│   └── Orders.csv
│
│── SQL/
│   ├── Create_Tables.sql
│   ├── Import_Data.sql
│   ├── Basic_Queries.sql
│   └── Business_Analysis.sql
│
├── README.md
```

---

# 🗄 Database Schema

The project contains three relational tables.

## 📖 Books

Stores information about available books.

| Column         | Description         |
| -------------- | ------------------- |
| Book_ID        | Primary Key         |
| Title          | Book Name           |
| Author         | Author Name         |
| Genre          | Book Category       |
| Published_Year | Publication Year    |
| Price          | Book Price          |
| Stock          | Available Inventory |

---

## 👤 Customers

Stores customer information.

| Column      | Description    |
| ----------- | -------------- |
| Customer_ID | Primary Key    |
| Name        | Customer Name  |
| Email       | Email Address  |
| Phone       | Contact Number |
| City        | City           |
| Country     | Country        |

---

## 🛒 Orders

Stores all purchase transactions.

| Column       | Description     |
| ------------ | --------------- |
| Order_ID     | Primary Key     |
| Customer_ID  | Foreign Key     |
| Book_ID      | Foreign Key     |
| Order_Date   | Purchase Date   |
| Quantity     | Books Purchased |
| Total_Amount | Order Value     |

---

# 🔗 Database Relationships

```
Customers
    │
    │
    ▼
 Orders
    ▲
    │
Books
```

* One Customer → Many Orders
* One Book → Many Orders
* Orders table connects Customers and Books

---

# 📥 Data Import

CSV files were imported into PostgreSQL using the **COPY** command.

* Books.csv
* Customers.csv
* Orders.csv

---

# 📊 SQL Analysis Performed

## Basic SQL Queries

* Retrieve books by genre
* Filter books by publication year
* Find books within a price range
* Identify customers by country
* Retrieve orders within a date range
* Calculate total inventory
* Find the most expensive book
* Identify low-stock books
* Calculate total revenue

---

# 📈 Business Analysis Queries

### 📚 Total Books Sold by Genre

Used **JOIN**, **SUM()**, and **GROUP BY** to determine the best-performing genres.

---

### 💰 Average Price by Genre

Analyzed pricing trends using the **AVG()** function.

---

### 👥 Repeat Customers

Identified customers placing multiple orders using **GROUP BY** and **HAVING**.

---

### 🔥 Most Frequently Ordered Books

Ranked books based on customer demand using **COUNT()** and **ORDER BY**.

---

### ✍️ Author Performance

Calculated total quantity sold for each author.

---

### 💵 Highest Spending Customers

Used **SUM()** aggregation to identify customers generating maximum revenue.

---

### 📦 Inventory Remaining

Calculated remaining stock after completed orders using:

* LEFT JOIN
* COALESCE()
* Aggregate Functions

---

# 📊 Business Insights

* Certain book genres generate significantly higher sales.
* A small number of books contribute to most of the total revenue.
* Repeat customers play an important role in overall sales.
* Inventory analysis helps identify books that require restocking.
* Customer spending analysis highlights high-value customers.
* Sales trends can support pricing and inventory decisions.

---

# 🧠 SQL Concepts Demonstrated

* Database Design
* Primary Keys
* Foreign Keys
* INNER JOIN
* LEFT JOIN
* GROUP BY
* HAVING
* ORDER BY
* Aggregate Functions
* CASE Statements
* Filtering
* Date Functions
* Subqueries
* Inventory Calculations
* Business Reporting

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

### 3️⃣ Create Tables

Execute the table creation script.

### 4️⃣ Import CSV Files

Import all datasets using the PostgreSQL COPY command.

### 5️⃣ Execute SQL Queries

Run the SQL scripts to generate business reports and insights.

---

# 🎯 Learning Outcomes

Through this project, I strengthened my understanding of:

* Relational Database Design
* SQL Query Optimization
* Business-Oriented Data Analysis
* Data Aggregation
* Reporting & Decision Support
* PostgreSQL Database Management

---

# 📸 Project Preview

> Add screenshots here showing:
>
> * Database Tables
> * ER Diagram (optional)
> * SQL Query Results
> * PostgreSQL Output
> * Execution Screenshots

---

# ⭐ Repository Features

* Clean SQL Scripts
* Structured Database Design
* Beginner-Friendly
* Real-World Business Questions
* Interview-Oriented SQL Practice
* Well Documented

---

# 👨‍💻 Author

**Sanjay Chourasiya**

**Aspiring Data Analyst**

**Skills:** SQL • PostgreSQL • Excel • Power BI • Python

If you found this project helpful, consider giving it a ⭐ on GitHub.
