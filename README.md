<p align="center"> <img src="https://placehold.co/1000x300/0f172a/38bdf8?text=DATA+DIGGER+2.0&font=montserrat" width="100%" alt="Data Digger Banner"> </p>

<p align="center"> <img src="https://img.shields.io/badge/SQL-MySQL-blue?style=for-the-badge&logo=mysql&logoColor=white" alt="MySQL"> <img src="https://img.shields.io/badge/Project-Data%20Analytics-green?style=for-the-badge" alt="Data Analytics"> <img src="https://img.shields.io/badge/Author-Arpit%20Shukla-orange?style=for-the-badge" alt="Author"> </p>

🚀 About the Project
Data Digger 2.0 is a MySQL-based database management project created by Arpit Shukla. It demonstrates essential SQL operations and data analysis using four relational tables: Customers, Orders, Products, and OrderDetails.

🎬 Coding Animation
<p align="center"> <img src="https://media.giphy.com/media/L8K62iTDkzGX6/giphy.gif" width="400" alt="Coding Animation"> </p>

🛠️ Technologies Used
MySQL
SQL
Relational Database Management
Data Analysis
🗂️ Database Structure
Table Name	Description
Customers	Stores customer names, emails, and addresses
Orders	Stores order IDs, dates, customer IDs, and amounts
Products	Stores product names, prices, and stock quantities
OrderDetails	Stores order items, quantities, and subtotals
🔗 Table Relationships
Customers.CustomerID → Orders.CustomerID
Orders.OrderID → OrderDetails.OrderID
Products.ProductID → OrderDetails.ProductID
✨ Key Features
Create and manage databases and tables
Insert, update, and delete records
Search customers by name
Filter records using WHERE and BETWEEN
Sort products by price using ORDER BY
Calculate revenue using SUM()
Find maximum, minimum, and average order amounts
Analyze product quantities using GROUP BY
Retrieve related records using JOIN
Find the most expensive and cheapest products using subqueries
Retrieve recent orders using date functions
Find the top three products by quantity sold
💻 SQL Query Examples
1. Calculate Total Revenue
SELECT SUM(SubTotal) AS TotalRevenue
FROM OrderDetails;
2. Find the Most Expensive Product
SELECT *
FROM Products
WHERE Price = (
    SELECT MAX(Price)
    FROM Products
);
3. Find the Cheapest Product
SELECT *
FROM Products
WHERE Price = (
    SELECT MIN(Price)
    FROM Products
);
4. Retrieve Customer Orders
SELECT
    Customers.Name,
    Orders.OrderID,
    Orders.OrderDate,
    Orders.TotalAmount
FROM Customers
JOIN Orders
    ON Customers.CustomerID = Orders.CustomerID;
5. Find the Top 3 Products by Quantity
SELECT
    ProductID,
    SUM(Quantity) AS TotalQuantity
FROM OrderDetails
GROUP BY ProductID
ORDER BY TotalQuantity DESC
LIMIT 3;
6. Calculate Order Statistics
SELECT
    MAX(TotalAmount) AS HighestAmount,
    MIN(TotalAmount) AS LowestAmount,
    AVG(TotalAmount) AS AverageAmount
FROM Orders;
7. Find Orders from the Last 30 Days
SELECT *
FROM Orders
WHERE OrderDate >= CURDATE() - INTERVAL 30 DAY;
▶️ How to Run the Project
Install MySQL Server and MySQL Workbench.
Download or clone the project repository.
Open the SQL script in MySQL Workbench.
Execute the SQL statements in the correct order.
Run the SELECT queries to view the results.
⚠️ Important: The script begins with DROP DATABASE DataDigger2;. This permanently deletes the existing database with that name. Back up important data before running the script.

🖼️ Images and Resources
🐬 MySQL Official Website
📚 MySQL Documentation
🎞️ Coding Animation GIFs
🖼️ Database Banner Images
💻 Create a GitHub Repository
🎯 Learning Outcomes
Through this project, I practiced:

SQL fundamentals and CRUD operations
Database design and foreign-key relationships
Aggregate functions and grouping
Joins and subqueries
Filtering and sorting records
Basic sales and inventory analysis
👨‍💻 Author
Arpit Shukla

SQL | MySQL | Database Management | Data Analytics

<p align="center"> ⭐ If you find this project useful, don't forget to give it a star! </p>

GitHub par upload karne ke liye: 
Create a new repository  par jao, repository ka naam DataDigger2 rakho aur README.md mein upar wala content paste kar do.


# PR.1-Data-Digger
