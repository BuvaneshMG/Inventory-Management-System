# Inventory Management System

A MySQL-based Inventory Management System designed to manage products, suppliers, customers, employees, purchases, sales, and inventory. This project demonstrates database design using SQL with relationships, primary keys, foreign keys, and realistic sample data.

## Features

* Manage product categories
* Store supplier information
* Manage customers and employees
* Track products and stock quantities
* Record purchase orders
* Record customer sales
* Maintain inventory records
* Generate reorder alerts when stock is low

## Database Tables

* Categories
* Suppliers
* Employees
* Customers
* Products
* PurchaseOrders
* PurchaseDetails
* Sales
* SaleDetails
* Inventory
* ReorderAlerts

## Technologies Used

* MySQL
* SQL
* MySQL Workbench

## Database Design

The database uses:

* Primary Keys
* Foreign Keys
* AUTO_INCREMENT
* One-to-Many Relationships
* Relational Database Design

## How to Run

1. Open MySQL Workbench.
2. Create the database:

   ```sql
   CREATE DATABASE Inventory_Management;
   USE Inventory_Management;
   ```
3. Execute the table creation script.
4. Execute the data insertion script (`Inventory_Management_1000_Rows.sql`).
5. Run SQL queries to view and manage the data.

## Sample Queries

```sql
SELECT * FROM Products;

SELECT * FROM Customers;

SELECT * FROM Sales;

SELECT ProductName, StockQuantity
FROM Products
WHERE StockQuantity < ReorderLevel;

SELECT ProductName, SellingPrice
FROM Products
ORDER BY SellingPrice DESC;
```

## Project Structure

```
Inventory-Management-System/
│
├── Inventory_Management.sql
├── Inventory_Management_1000_Rows.sql
├── README.md
└── ER_Diagram.png (optional)
```

## Future Improvements

* Stored Procedures
* Triggers
* Views
* User Authentication
* Sales Reports
* Dashboard Integration

## Author

Developed as a MySQL database project for learning relational database design and SQL.
