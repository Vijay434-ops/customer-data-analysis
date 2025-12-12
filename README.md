# customer-data-analysis
End-to-End Customer Data Analysis using SQL &; Power  BI

🛒 Customer Data Analysis – End-to-End Data Analytics Project

This project focuses on analyzing customer shopping behavior using SQL and Power BI.
The goal is to identify key revenue-driving segments, product performance, and payment trends to provide actionable insights for business growth.


---

🚀 Project Objectives

1. Analyze shopping distribution according to gender
2. Identify which gender purchased more quantity
3. Determine which gender generated higher revenue
4. Analyze category distribution
5. Study shopping distribution across age groups
6. Identify which age group purchased more quantity
7. Determine which age group generated highest revenue
8. Analyze category variation across gender and age
9. Study relationship between payment method & other attributes
10. Analyze distribution of payment methods
11. Build interactive Power BI dashboard and provide insights




---

🗂️ Dataset Summary

Rows: 1000
Columns: Customer ID, Gender, Age, Category, Quantity, Price, Payment Method, Invoice No, Shopping Mall
Source: Provided by DataMites
Contains demographic information + purchase behavior



---

🛠️ Technologies Used

SQL (MySQL) – Data extraction & analysis
Power BI – Dashboard creation
Excel – Data cleaning
Python (optional) – Data inspection
GitHub – Version control & portfolio showcase



---

📊 Power BI Dashboard

👉 Add your dashboard image here:

![Dashboard](./PowerBI/Customer_Data_Analysis_Dashboard.png)

The dashboard includes:

Total Transactions
Total Revenue
Average Quantity
Average Order Value (AOV)
Gender-wise transactions & revenue
Age-wise transactions & revenue
Category performance
Payment method distribution
Slicers for Gender, Age Group, Category, Payment Method



---

🧮 SQL Analysis

All SQL queries are stored in:
/SQL/customer_data_analysis_queries.sql

Sample queries:

-- Shopping distribution by gender
SELECT gender, COUNT(*) AS total_transactions
FROM customer
GROUP BY gender;

-- Revenue by age group
SELECT 
 CASE 
  WHEN age BETWEEN 18 AND 25 THEN '18-25'
  WHEN age BETWEEN 26 AND 35 THEN '26-35'
  WHEN age BETWEEN 36 AND 45 THEN '36-45'
  WHEN age BETWEEN 46 AND 55 THEN '46-55'
  ELSE '56+'
 END AS age_group,
 SUM(quantity * price) AS total_revenue
FROM customer
GROUP BY age_group;


---

🔍 Key Insights

Female customers have higher transaction volume

Age group 36–55 generates the highest revenue

Clothing, Shoes & Accessories are top-performing categories

Credit Card is the most used payment method

Younger customers (18–25) show low engagement

Middle-aged customers (36–55) are ideal for targeted marketing



---

💡 Recommendations

Create targeted campaigns for female and middle-aged customers

Increase stock & promotions for top-selling categories

Improve visibility for low-performing categories

Launch card cashback or reward programs

Use customer segmentation for personalized marketing



---

📁 Project Files Included

File/Folder	Description

Dataset	Raw dataset used for analysis
SQL	All SQL queries used in the project
PowerBI	Dashboard file + PNG image
Report	Detailed project report (PDF)
Presentation	Final project PPT
README.md	GitHub documentation



---

📬 Contact

Vijay Raghavendra
📍 Karnataka, India
💼 Aspiring Data Analyst
📧 you can add your own email
