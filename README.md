# Data_Warehouse_SQL_Project
Data Warehouse with SQL Server, including ETL processes and data modelling.

## 🏗 Architecture & Workflow
![Medallion Architecture](https://github.com/Gunelhasan/Data_Warehouse_SQL_Project/blob/main/data_warehouse_medallion.png?raw=true)

- **Bronze** – Raw data storage (CSV imports).
- **Silver** – Cleaned, standardized and enriched data (data quality improvements).
- **Gold** – Business-ready data marts for analytics and reporting.

The data warehouse follows a **Star Schema** design in the Gold layer, optimized for analytical queries and business reporting.  
It includes **fact tables** for transactional data and **dimension tables** for descriptive attributes.

![Data Model](https://github.com/Gunelhasan/Data_Warehouse_SQL_Project/blob/main/data_modelling.jpg)

## 🛠 Tools & Technologies
- **SQL Server** (Database Engine)
- **SQL Server Management Studio (SSMS)**
- **ETL Process with T-SQL**
- **Dimensional Modeling** (Star Schema)
- **Data Warehouse Design Principles**
- **CSV to SQL Data Loading**
