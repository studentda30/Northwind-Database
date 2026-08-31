Northwind Database

A SQL Server implementation of the Northwind sample database, containing a complete relational database schema and sample business data.

This project is useful for learning and practicing SQL, database design, queries, joins, relationships, constraints, views, and data analysis.

📌 About the Database

Northwind is a classic sample database originally created by Microsoft for demonstrating relational database concepts.

The database represents a fictional company that sells products to customers and manages orders, suppliers, employees, shippers, and territories.

This repository contains the SQL script required to create and populate the Northwind database.

🗂️ Database Contents

The database includes tables such as:

Categories
Customers
Employees
EmployeeTerritories
Order Details
Orders
Products
Regions
Shippers
Suppliers
Territories

The tables are connected through primary keys and foreign keys, providing a realistic relational database structure.

🛠️ Technologies
Microsoft SQL Server
T-SQL
SQL Server Management Studio (SSMS)
📁 Project Structure
Northwind-Database/
│
├── instnwnd.sql
└── README.md

🚀 How to Install
1. Download the SQL file

Download instnwnd.sql from this repository.

2. Open SQL Server Management Studio

Open SQL Server Management Studio (SSMS) and connect to your SQL Server instance.

3. Open the SQL script

Open:

instnwnd.sql

4. Execute the script

Run the script in SSMS.

The script will create and populate the Northwind database.

5. Verify the database

After execution, refresh the Databases folder in SSMS.

You should see:

Northwind

🔗 Original Microsoft Source

This project is based on Microsoft's official Northwind sample database.

Microsoft Northwind SQL Script
Microsoft Northwind Documentation
Microsoft SQL Server Samples Repository
📊 What You Can Practice

This database is suitable for practicing:

SELECT
WHERE
ORDER BY
GROUP BY
HAVING
JOIN
INNER JOIN
LEFT JOIN
RIGHT JOIN
Subqueries
Common Table Expressions (CTEs)
Aggregate functions
Window functions
Primary keys
Foreign keys
Constraints
Views
Stored procedures
Data analysis
💡 Example Query

Find the top 10 products by quantity sold:

SELECT TOP 10
    p.ProductName,
    SUM(od.Quantity) AS TotalQuantity
FROM Products p
JOIN [Order Details] od
    ON p.ProductID = od.ProductID
GROUP BY p.ProductName
ORDER BY TotalQuantity DESC;

🎯 Purpose

The purpose of this repository is to provide a simple environment for learning and practicing SQL and relational database concepts using a realistic sample dataset.

📜 Source

Northwind is a Microsoft sample database. The original SQL Server sample scripts are maintained in Microsoft's SQL Server Samples repository.

⭐ If You Find This Useful

Feel free to ⭐ star the repository and use the database for your SQL learning and practice.
