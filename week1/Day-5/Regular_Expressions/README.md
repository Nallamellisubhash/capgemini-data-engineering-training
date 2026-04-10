

##  Overview
This project focuses on understanding and applying **Regular Expressions (REGEX)** using SQL and PySpark for data extraction, validation, and transformation.

The dataset used contains structured and semi-structured fields such as:
- Emails
- Phone numbers
- Mixed alphanumeric values
- Pattern-based text fields

The goal is to extract meaningful information from complex strings using REGEX.

---

##  Objectives
- Learn fundamentals of REGEX from basics
- Apply REGEX in SQL queries
- Perform pattern-based data extraction
- Validate real-world data formats
- Clean and transform messy datasets

---

## 🛠️ Technologies Used
- PySpark 


---

##  Dataset Description

The dataset includes the following columns:

- **id** → Unique identifier  
- **full_text** → Pattern-based values (EMP, USR, ORD, LOG formats)  
- **email** → Email addresses with different domains  
- **phone** → Phone numbers with country codes  
- **mixed_value** → Combination of alphabets and numbers  

---

##  Key Concepts Covered

###  Regex Fundamentals
- Character sets `[0-9]`, `[A-Za-z]`
- Anchors `^` (start), `$` (end)
- Quantifiers `+`, `{n}`, `?`
- Continuity principle

---

###  Data Extraction
- Extract digits from start and end
- Extract alphabets and numeric parts
- Extract substrings from the middle
- Extract last characters and patterns

---

###  Email Processing
- Extract username (before `@`)
- Extract domain name
- Extract extension (`.com`, `.in`)
- Validate email format using regex

---

###  Phone Number Handling
- Extract country code
- Handle multiple formats (+91, 91, etc.)
- Clean unwanted characters

---

###  Pattern-Based Extraction
- Extract employee numbers from text
- Extract digits between alphabets
- Extract exact number of characters
- Work with structured patterns like:
  - EMP001_IN_91
  - ORD-11-IN
  - LOG91DATA

---

##  Real-World Applications
- Data cleaning in ETL pipelines
- Validating user input (email, phone)
- Log data processing
- Preparing datasets for analytics
- Handling messy real-world data

---

##  Learning Outcomes
By completing this project, you will:
- Gain strong understanding of REGEX concepts
- Apply regex in SQL and PySpark
- Handle real-world string data efficiently
- Improve data transformation skills
- Build a foundation for data engineering roles

---

##  Conclusion
Regex is a powerful tool for working with text data. This project demonstrates how REGEX can be used effectively in SQL and PySpark to extract, validate, and clean data in real-world scenarios.

