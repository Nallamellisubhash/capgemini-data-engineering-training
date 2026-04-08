# SQL Practice – Window Functions

##  Overview

This project demonstrates the use of **Window Functions** in SQL for advanced data analysis. It focuses on performing calculations across a set of rows while retaining individual row details.

---

##  Definition

Window functions are used to perform calculations across a group of rows related to the current row without collapsing the result into a single row.

---

##  Purpose

* Analyze data without losing row-level details
* Perform ranking and ordering
* Calculate running totals and cumulative values
* Compare values between rows

---

##  Key Concepts

### 1. Partitioning

* Divides data into groups
* Similar to GROUP BY, but does not reduce rows

---

### 2. Ordering

* Defines the sequence of rows within each partition
* Used for ranking and cumulative calculations

---

### 3. Window Clause

* Defines how the window is formed
* Uses PARTITION BY and ORDER BY

---

##  Types of Window Functions

### 1. Aggregate Functions

* Used with window clause
* Examples: total, average, count per group

---

### 2. Ranking Functions

* Assign ranks to rows
* Used for ordering and comparison

---

### 3. Value Functions

* Access values from other rows
* Useful for comparisons and trend analysis

---

##  Use Cases

* Ranking employees by salary
* Finding top performers
* Calculating running totals
* Comparing current row with previous or next row
* Department-wise analysis without grouping

---

##  Important Points

* Window functions do not reduce rows
* Executed after GROUP BY and HAVING
* Cannot be used directly in WHERE or HAVING
* Often used with subqueries or CTEs

---

##  Difference from GROUP BY

* GROUP BY → reduces rows
* Window Functions → retain all rows

---

##  Summary

Window functions are powerful tools for analytical queries, allowing complex calculations while preserving detailed data.


