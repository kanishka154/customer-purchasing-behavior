🛍️ Customer Purchasing Behavior Analysis
A data analysis project exploring customer purchasing patterns using Python and pandas — covering data cleaning, aggregation, and pivot table analysis.

📌 Project Overview
This project analyzes a real-world customer dataset to uncover insights about purchasing behavior across regions, age groups, income levels, and loyalty categories. The analysis is structured in three phases: Data Cleaning → GroupBy & Aggregation → Pivot Tables.

📂 Dataset
File: Customer Purchasing Behaviors.csv
Column                  Description
user_id                  Unique customer identifier
age                      Customer age
annual_income            Annual income (in ₹/USD)
purchase_amount          Amount spent per transaction
loyalty_score            Score between 0–10
region                   Geographic region
purchase_frequency       Number of purchases

🔧 Phase 1 — Data Cleaning

Checked and handled null/missing values using median/mode imputation
Removed duplicate rows
Filtered out unrealistic age values (e.g., 0 or 200+)
Validated loyalty_score range (0–10)
Verified and corrected data types for all numerical columns
Detected outliers in purchase_amount and annual_income using the IQR method

📊 Phase 2 — GroupBy & Aggregation
Key questions answered:

Average purchase amount per region
Customer count by region
Average loyalty score by age group (20–29, 30–39, 40–49, 50+)
Region with highest average purchase frequency
Max/min annual income per region
Loyalty segmentation: Low (0–4), Medium (4–7), High (7–10)
Total purchase amount by age group
Income group comparison: Low Income (<50K) vs High Income (≥50K)

📋 Phase 3 — Pivot Tables
Pivot           Description

P1               Region-wise average purchase amount
P2               Age group × Region — average loyalty score
P3               Income group × Region — total purchase amount
P4               Loyalty category × Region — customer count
P5               Region-wise summary with grand totals

🛠️ Tools & Libraries

Python 3.x
pandas
numpy
Jupyter Notebook

🚀 How to Run

# 1. Clone the repository
git clone https://github.com/kanishka154/customer-purchasing-behavior.git

# 2. Install dependencies
pip install pandas numpy jupyter

# 3. Open the notebook
jupyter notebook 11__CUSTOMER_PURCHASING_BEHAVIOUR.ipynb

💡 Key Insights

Customers in different regions show significantly different average purchase amounts
Higher loyalty scores do not always correlate with higher income groups
The IQR method revealed measurable outliers in both income and purchase columns
Age group 30–39 shows the highest average loyalty engagement

👩‍💻 Author
Kanishka Joshi
BCom Student | Data Science & AI Enthusiast
📍 Delhi, India
https://linkedin.com/in/kanishkajoshi1
