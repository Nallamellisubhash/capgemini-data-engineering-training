In this task, I worked with sales and customer data using PySpark.
I focused on cleaning the data, calculating total spend, and applying different methods to segment customers.
 What I Did
Cleaned the data by removing null values, duplicates, and invalid records
Joined sales and customer datasets
Created a full name column using first and last name
Calculated total spend for each customer



🔹 Segmentation Methods Used
1. Rule-Based Segmentation
Used fixed conditions:
Gold → high spend
Silver → medium spend
Bronze → low spend
2. Quantile-Based Segmentation
Used approxQuantile() to divide customers based on data distribution
Automatically created segments based on percentiles
3. Rank-Based Segmentation (Window Function)
Used percent_rank() to rank customers
Assigned segments based on ranking percentage
4. Bucketizer Method
Used predefined ranges (bins)
Converted spend values into buckets and mapped them to segments


 Final Comparison
Compared all segmentation methods in one table
Observed how different techniques classify customers differently


 Key Learnings
Data cleaning is very important before analysis
There are multiple ways to segment customers
Window functions and Bucketizer are powerful tools
Different methods give different business insights
