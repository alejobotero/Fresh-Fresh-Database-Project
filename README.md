# Farmers Market Database Project

This project involves designing and developing a comprehensive database system for managing farmers market data, including conceptual design, normalization, and implementation in SQL. The system supports efficient data retrieval, manipulation, and integrity maintenance.

## Features
- **Conceptual Design**: ER diagram for farmers market operations.
- **Database Normalization**: Pre-normalization, 1NF, 2NF, and 3NF schema design.
- **SQL Implementation**: Scripts for schema creation, queries, and data manipulation.
- **Data Analysis**: Example queries for business insights.

## Directory Structure
- **`sql/`**: SQL scripts for schema creation and sample queries.
- **`data/`**: Raw and normalized sample data in CSV format.
- **`diagrams/`**: ER diagram and relational schema.
- **`excel/`**: Example Excel file for data analysis.

## ER Diagram
![image](https://github.com/user-attachments/assets/e95189c6-ce9f-488e-b01d-ceebfee4c268)

## Example Queries
- **Retrieve All Produce by Category**:
  ```sql
  SELECT Category, Product
  FROM Produce
  JOIN Category ON Produce.CategoryID = Category.CategoryID;
