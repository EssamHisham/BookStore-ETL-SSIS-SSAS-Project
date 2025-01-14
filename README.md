# Gravity Bookstore Data Warehouse Project

## Project Overview

This project involves modeling and building a data warehouse for a fictional bookstore, Gravity Bookstore. The goal is to capture and analyze information about books, customers, and sales through a well-structured data warehouse. The project includes the creation of a data warehouse, ETL processes using SQL Server Integration Services (SSIS), and OLAP cube development using SQL Server Analysis Services (SSAS).

## Use Case Background

Gravity Bookstore is a fictional database that captures essential information about books, customers, and sales. The database includes various tables that represent the relationships between books, authors, customers, and orders.

### Database Structure

The `gravity_books` transactional database consists of the following tables:

- **book**: A list of all books available in the store.
- **book_author**: Stores the authors for each book, representing a many-to-many relationship.
- **author**: A list of all authors.
- **book_language**: A list of possible languages for the books.
- **publisher**: A list of publishers for the books.
- **customer**: A list of customers of Gravity Bookstore.
- **customer_address**: A list of addresses for customers, as a customer can have multiple addresses.
- **address_status**: A list of statuses for addresses (current or old).
- **address**: A list of addresses in the system.
- **country**: A list of countries associated with the addresses.
- **cust_order**: A list of orders placed by customers.
- **order_line**: A list of books included in each order.
- **shipping_method**: Possible shipping methods for an order.
- **order_history**: The history of an order (e.g., ordered, cancelled, delivered).
- **order_status**: Possible statuses of an order.

## Project Requirements

1. **Data Warehouse Development**: 
   - Model and develop the `gravity_books_dwh` Data Warehouse.
   - Provide DDL statements for table creation and a screenshot of the DWH diagram (Dimensional Modeling).

2. **Schema Approach**: 
   - Define the approach used for the data warehouse (star schema or snowflake) and explain the rationale behind the choice.

3. **Data Integrity**: 
   - Define a method to check and maintain the integrity between the fact and dimension tables using SQL.

4. **Date Dimension**: 
   - Add a date dimension to the system to track historical changes.

5. **ETL Process**: 
   - Design an SSIS project to populate data from the `gravity_books` transactional database into the `gravity_books_dwh` data warehouse.

6. **OLAP Cube Development**: 
   - Design an SSAS project (multidimensional model) and provide the main deliverables for cube browsing.

## Deliverables

- DDL statements for the data warehouse (`format.sql`)
- ETL SSIS project files
- OLAP SSAS project files
- Mapping sheet
- Screenshots of outputs for each requirement

## Getting Started

To get started, please download the SQL files from the following link and run them in a new database named `gravity_books` in your local SQL Server DB engine:

[Gravity SQL Server Database on GitHub](https://github.com/databasestar/sample_databases/sample_db_gravity/gravity_sqlserver)

## Screenshots

Please refer to the repository for screenshots of the outputs for each requirement.

![DWH PROJECT1](https://github.com/EssamHisham/GravityBooks-ETL-SSIS-SSAS-Project/blob/master/ScreenCaptures/DWH%20PROJECT1.jpeg?raw=true)
![DWH PROJECT7](https://github.com/EssamHisham/GravityBooks-ETL-SSIS-SSAS-Project/blob/master/ScreenCaptures/DWH%20PROJECT7.jpeg?raw=true)
