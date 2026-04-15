#  PySpark Data Pipeline Project (Day 3 – BSG)

##  Project Overview
This project demonstrates a basic data engineering pipeline using PySpark, following a layered architecture approach (Bronze → Silver → Gold).

It focuses on data ingestion, cleaning, transformation, and generating business insights from sales data.

---

##  Technologies Used
- Python
- PySpark
- Spark SQL

---

##  Dataset Description

The dataset contains sales transaction data with the following fields:

- order_id → Unique order identifier  
- customer_id → Customer ID  
- product → Product name  
- category → Product category  
- city → Customer city  
- date → Order date  
- amount → Transaction amount  
- quantity → Quantity purchased  

---

##  Architecture

###  Bronze Layer (Raw Data)
- Raw data ingestion
- Contains duplicates, null values, and invalid data

###  Silver Layer (Cleaned Data)
- Data cleaning and preprocessing
- Removed duplicates
- Handled null values
- Filtered invalid records

###  Gold Layer (Business Insights)
- Aggregated data for analysis
- Prepared data for reporting and dashboards

---

##  Data Issues Handled

- Duplicate records
- Missing values
- Invalid transaction amounts
- Inconsistent data

---

##  Key Insights Generated

- Top selling products
- High-value customers
- Revenue by city
- Product performance analysis

---

##  Learning Outcomes

- Understanding ETL pipeline in PySpark
- Working with structured data
- Data cleaning techniques
- Data aggregation concepts
- Real-world data processing workflow

---

##  Future Improvements

- Integration with Delta Lake
- Incremental data loading
- Advanced analytics using window functions
- Dashboard creation using BI tools

