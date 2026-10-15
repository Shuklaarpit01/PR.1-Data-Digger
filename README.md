 
<div align="center">

# 🚀 PR.1 DATA DIGGER 🚀

### 🗄️ SQL Database Management Project

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=25&pause=1000&color=00C9FF&center=true&vCenter=true&width=600&lines=Welcome+to+Data+Digger!;Explore+SQL+Queries;Manage+Your+Database;Learn+MySQL+Step+by+Step" alt="Animated typing banner" />

![MySQL](https://img.shields.io/badge/MySQL-Database-blue?style=for-the-badge&logo=mysql&logoColor=white)
![SQL](https://img.shields.io/badge/Language-SQL-orange?style=for-the-badge&logo=databricks&logoColor=white)
![Project](https://img.shields.io/badge/Project-Data%20Digger-purple?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

**✨ Discover Data • Write Queries • Analyze Results ✨**

</div>

---

## 📌 About the Project

**Data Digger** is a SQL database management project created to practice basic and intermediate SQL commands using MySQL.

This project demonstrates how to create databases and tables, insert records, update and delete data, filter information, perform calculations, and combine data from multiple tables using joins.

## 🎯 Project Objectives

- Learn database and table creation.
- Insert, update, and delete records.
- Retrieve data using `SELECT` queries.
- Filter and sort records.
- Perform aggregate calculations.
- Understand primary keys and foreign keys.
- Use joins and subqueries to analyze data.

## 🛠️ Technologies Used

- **Database:** MySQL
- **Language:** SQL
- **Editor:** MySQL Workbench / Visual Studio Code with a MySQL extension

## 🗂️ Database Structure

The project contains four tables:

| Table | Description |
|---|---|
| `Customers` | Stores customer names, emails, and addresses |
| `Orders` | Stores order dates, customer IDs, and order amounts |
| `Products` | Stores product names, prices, and stock |
| `OrderDetails` | Stores ordered products, quantities, and subtotals |

## ⚡ SQL Concepts Covered

### 1. Database Operations
- `CREATE DATABASE`
- `DROP DATABASE`
- `USE`

### 2. Table and Data Operations
- `CREATE TABLE`
- `INSERT INTO`
- `UPDATE`
- `DELETE`

### 3. Data Retrieval
- `SELECT`
- `WHERE`
- `ORDER BY`
- `BETWEEN`
- `LIMIT`

### 4. Aggregate Functions
- `MAX()`
- `MIN()`
- `AVG()`
- `SUM()`
- `COUNT()`

### 5. Advanced SQL Queries
- Primary and foreign keys
- `INNER JOIN`
- Subqueries
- `GROUP BY`
- Date filtering with `CURDATE()` and `INTERVAL`

## 💻 Example SQL Queries

**Find all customers:**

```sql
SELECT * FROM Customers;
```

**Find the most expensive product:**

```sql
SELECT *
FROM Products
WHERE Price = (
    SELECT MAX(Price)
    FROM Products
);
```

**Calculate total revenue from order details:**

```sql
SELECT SUM(SubTotal) AS TotalRevenue
FROM OrderDetails;
```

**Join customers with their orders:**

```sql
SELECT
    Customers.Name,
    Orders.OrderID,
    Orders.OrderDate,
    Orders.TotalAmount
FROM Customers
JOIN Orders
ON Customers.CustomerID = Orders.CustomerID;
```

## 📊 Expected Learning Outcomes

After completing this project, you will understand how to:

- Organize data in relational tables.
- Maintain relationships between tables.
- Retrieve specific records with SQL queries.
- Calculate totals, averages, minimums, and maximums.
- Analyze customer orders and product information.

## ▶️ How to Run the Project

1. Install MySQL Server.
2. Open MySQL Workbench or connect to MySQL from VS Code.
3. Open a new SQL query editor.
4. Copy the SQL script into the editor.
5. Execute the script in order.
6. Run the `SELECT` queries to view the results.

**⚠️ Important:** The script starts with `DROP DATABASE DataDigger2;`, which deletes the existing database with that name and its contents. Remove or comment out that line if you want to preserve existing data.

## 👨‍💻 Author

**Shukla Arpit**

SQL Practice Project — PR.1 Data Digger

---

<div align="center">

### 🌟 Thanks for Visiting My Project! 🌟

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=20&pause=1000&color=F7971E&center=true&vCenter=true&width=500&lines=Keep+Learning!;Keep+Practicing!;Keep+Growing!;Happy+Coding+%F0%9F%9A%80" alt="Animated closing message" />

**💙 Keep Exploring the World of SQL! 💙**

</div>
