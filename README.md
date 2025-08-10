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


<br><br>
**Working in SQL Server**

Here’s an example of my workflow while creating the `gold.dim_customers` view in SSMS:

![SQL Server Screenshot](sql%20ekran.png)

<br><br>

**Sales Data Mart – Star Schema**

After transforming and loading the data into the **Gold Layer**,  
I designed a **Star Schema** to organize the Sales Data Mart for analytical purposes.

The schema consists of:

- **Fact Table**: `gold.fact_sales` – stores transaction details such as order dates, quantities, prices, and amounts.
- **Dimension Tables**:
  - `gold.dim_customers` – customer profile data
  - `gold.dim_productss` – product information

**Primary Keys (PK)** uniquely identify each row in dimension tables,  
and **Foreign Keys (FK)** link the fact table to its related dimensions.

![Sales Data Mart Star Schema](https://github.com/Gunelhasan/Data_Warehouse_SQL_Project/blob/main/SalesDataMart.drawio.png?raw=true)


## 🛠️ Important Links & Tools
Everything I used in this project is free and publicly available.

- **[Datasets](https://github.com/Gunelhasan/Data_Warehouse_SQL_Project/tree/main/dataset)** – CSV files used as the raw source data.
- **[SQL Server Express](https://www.microsoft.com/en-us/sql-server/sql-server-downloads)** – Lightweight version of SQL Server for hosting the database.
- **[SQL Server Management Studio (SSMS)](https://learn.microsoft.com/en-us/sql/ssms/download-sql-server-management-studio-ssms)** – GUI for managing and querying the SQL Server database.
- **[GitHub Repository](https://github.com/Gunelhasan/Data_Warehouse_SQL_Project)** – Version control and collaboration.
- **[Draw.io](https://app.diagrams.net/)** – For designing data architecture, star schema, and diagrams.
- **[Notion](https://www.notion.so/)** – For project planning and documentation.

  
<br><br>
  **This repository showcases expertise in:**
  <p align="center">
  <img src="https://img.shields.io/badge/SQL%20Development-00758F?style=for-the-badge&logo=Microsoft-SQL-Server&logoColor=white">
  <img src="https://img.shields.io/badge/Data%20Architecture-4B8BBE?style=for-the-badge&logo=databricks&logoColor=white">
  <img src="https://img.shields.io/badge/ETL%20Pipelines-F7931E?style=for-the-badge&logo=apache-airflow&logoColor=white">
  <img src="https://img.shields.io/badge/Data%20Modeling-006272?style=for-the-badge&logo=databricks&logoColor=white">
  <img src="https://img.shields.io/badge/Data%20Analytics-FF6F00?style=for-the-badge&logo=Power-BI&logoColor=white">
</p>


- **SQL Development** – writing complex queries, joins, aggregations, and optimizations.
- **Data Architecture** – designing a scalable Medallion architecture (Bronze–Silver–Gold layers).
- **Data Engineering** – building structured pipelines from raw ingestion to analytics-ready data.
- **ETL Pipeline Development** – implementing extraction, transformation, and loading processes using T-SQL.
- **Data Modeling** – designing a Star Schema with fact and dimension tables for analytical workloads.
- **Data Analytics** – creating queries and KPIs to support business decision-making.
