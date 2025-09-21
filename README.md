# Hardware-Appliances-Sales
The Sales.sql file is analysing the sale of the Hardware with different tables like Customers,Products,Orders,Ordersdetails.

# Sales Database
This project contains a **Sales Database** built using **MySQL**. It is designed to store and analyze customer and sales-related information, which can be further used for reporting and dashboard creation (e.g., in Power BI or Tableau).

## Features
* **Customers Table**: Stores customer details like name, age, gender, city, state, and phone.
* **Sales Data** (extendable): Can be linked with products, orders, and transactions for full analysis.
* **Preloaded Data**: Includes sample entries for quick testing and learning.

## Project Structure
* `Sales.sql` → MySQL script to create database and insert sample data.
* Tables included:
  * **Customers** (basic customer details)
  * *(extendable with Products, Orders, Transactions if required)*

## Example Queries
   sql
   Find total customers by state
SELECT State, COUNT(*) AS Total_Customers
FROM Customers
GROUP BY State;

   Gender distribution
SELECT Gender, COUNT(*) AS Total
FROM Customers
GROUP BY Gender;

   Average customer age
SELECT AVG(Age) AS Average_Age FROM Customers;

## How to Use
1. Open MySQL Workbench or CLI.
2. Run the script:

      sql
   SOURCE Sales.sql;
   
3. Explore tables using:
      sql
   SHOW TABLES;
   DESCRIBE Customers;
  
4. Start querying and analyzing data!
   
## Possible Extensions
* Add Orders, Products, and Transactions tables for sales analytics.
* Build a Power BI dashboard connected to the MySQL database.
* Perform data visualization like top states, revenue trends, and customer demographics.

This project is great for beginners learning MySQL and for anyone wanting to practice SQL queries on a sales dataset.
