#  Insurance Data Analysis using PySpark & SQL

##  Project Overview

This project focuses on analyzing insurance data using **PySpark and SQL** to identify customer risk, validate data quality, and generate meaningful business insights.

The dataset includes:

* Customers
* Policies
* Claims
* Agents
* Policy-Agent Mapping

---

##  Objectives

* Perform data understanding and cleaning
* Build relationships between datasets
* Compute key business metrics
* Identify high-risk customers
* Apply advanced SQL (CTE & Window Functions)

---

##  Phase-wise Implementation

###  Phase 1 – Data Understanding

* Loaded all datasets using PySpark
* Checked schema using `printSchema()`
* Validated row counts
* Identified:

  * Null values
  * Negative values
  * Invalid keys
* Understood relationships:

  ```
  Customer → Policy → Claim → Agent
  ```

---

###  Phase 2 – Data Cleaning

* Handled null values using `fillna()` and `dropna()`
* Removed negative values:

  * `premium < 0`
  * `claim_amount < 0`
* Standardized string columns using:

  * `trim()`
  * `initcap()`
* Ensured correct data types (dates, numeric)
* Removed invalid joins using referential checks

---

###  Phase 3 – Transformations

* Computed:

  * Total premium per customer
  * Total claims per customer
  * Risk score:

    ```
    risk_score = total_claim / total_premium
    ```
* Created city-wise aggregations

---

###  Phase 4 – SQL Analysis

* Used SQL for business queries:

  * Top customers per city
  * Repeat customers
  * Monthly trends

---

###  Phase 5 – Advanced SQL (CTE)

* Used `WITH` clause to break complex logic:

  * Premium aggregation
  * Claims aggregation
  * Risk computation
* Identified:

  * Top 3 risky customers per city
  * Customers with increasing claims (MoM)

---

###  Phase 6 – Window Functions

* Used:

  * `ROW_NUMBER()`
  * `RANK()`
  * `DENSE_RANK()`
* Ranked:

  * Agents based on premium handled
  * Customers based on risk score
* Applied `PARTITION BY city` for group ranking

---

###  Phase 7 – Final Output

* Created final unified dataset
* Added derived columns (e.g., risk flag)
* Saved output in:

  * CSV
  * Parquet (recommended)

---

##  Data Validation

* Compared row counts before and after joins
* Checked null values post-cleaning
* Ensured no duplicate records
* Verified referential integrity

---

##  Key Insights

* Identified high-risk customers (high claim vs premium)
* Detected claim trends using time-based analysis
* Found top-performing agents
* Analyzed city-wise business performance

---

##  Technologies Used

* **PySpark** → Data processing
* **SQL** → Analysis (CTE, Window Functions)
* **Parquet** → Efficient storage format

---



##  Conclusion

This project demonstrates end-to-end data engineering and analysis workflow including data cleaning, transformation, validation, and advanced analytics using PySpark and SQL.

---
