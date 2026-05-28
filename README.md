🛒 Customer Shopping Behavior Analysis
End-to-End Data Analytics Project | Python · SQL · Power BI
![Python](https://img.shields.io/badge/Python-3.10-blue?style=for-the-badge&logo=python&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-SQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![PowerBI](https://img.shields.io/badge/Power_BI-Dashboard-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Pandas](https://img.shields.io/badge/Pandas-Data_Cleaning-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)
---
📖 About the Project
This is a complete, industry-standard, end-to-end data analytics project that simulates the real workflow of a professional data analyst. It analyzes 3,900 customer transactions across multiple product categories to uncover insights into spending patterns, customer segments, product preferences, and subscription behavior.
The project covers every stage of the analytics pipeline — from raw data cleaning in Python, to SQL-based business analysis, to an interactive Power BI dashboard, and a final business report with recommendations.
---
❓ Business Problem
> *"How can the company leverage consumer shopping data to identify trends, improve customer engagement, and optimize marketing and product strategies?"*
A retail company noticed changes in purchasing patterns across demographics, product categories, and sales channels. They needed data-driven answers to improve sales, customer satisfaction, and long-term loyalty.
---
📁 Project Structure
```
customer-trends-analysis/
│
├── 📓 Customer_Shopping_Behavior_Analysis.ipynb    # Python EDA & data cleaning
├── 🗄️  customer_behavior_sql_queries.sql           # 10 SQL business queries
├── 📊 customer_behavior_dashboard.pbix             # Power BI interactive dashboard
├── 📄 customer_shopping_behavior.csv               # Raw dataset (3,900 rows)
├── 📋 Customer Shopping Behavior Analysis.pdf      # Full project report
└── 📑 Business Problem Document.pdf               # Business context & deliverables
```
---
🔄 Project Workflow
```
Raw Dataset (3,900 rows · 18 columns)
            ↓
🐍 Python (Jupyter Notebook)
   • Data Loading & Exploration
   • Missing Value Imputation (37 nulls in Review Rating)
   • Feature Engineering (age_group, purchase_frequency_days)
   • Column Standardization (snake_case)
   • Load cleaned data → PostgreSQL
            ↓
🗄️ SQL (PostgreSQL)
   • 10 Business Queries
   • Revenue Analysis, Customer Segmentation
   • Discount & Subscription Analysis
            ↓
📊 Power BI
   • Interactive Dashboard
   • KPI Cards, Bar Charts, Donut Charts
   • Filters by Gender, Category, Shipping, Subscription
            ↓
📋 Report & Business Recommendations
```
---
📊 Dataset Overview
Feature	Detail
Total Records	3,900 transactions
Total Columns	18 features
Missing Data	37 null values in Review Rating (imputed using category median)
Customer Demographics	Age, Gender, Location, Subscription Status
Purchase Details	Item, Category, Purchase Amount, Season, Size, Color
Behavior Features	Discount Applied, Previous Purchases, Frequency, Review Rating, Shipping Type
---
🐍 Python — Data Cleaning & EDA
Key steps performed in the Jupyter Notebook:
Data Loading — Imported dataset using `pandas`
Initial Exploration — Used `df.info()` and `.describe()` for structure & summary stats
Missing Data Handling — Imputed 37 null values in `review_rating` using median per product category
Column Standardization — Renamed all columns to `snake_case`
Feature Engineering:
Created `age_group` column by binning customer ages
Created `purchase_frequency_days` column from purchase data
Data Consistency Check — Found `discount_applied` and `promo_code_used` were redundant; dropped `promo_code_used`
Database Integration — Connected Python to PostgreSQL and loaded the cleaned DataFrame for SQL analysis
---
🗄️ SQL — Business Analysis (10 Queries)
Performed structured analysis in PostgreSQL to answer real business questions:
#	Business Question	Key Finding
1	Revenue by Gender	Male: $157,890 · Female: $75,191
2	High-Spend Discount Users	839 customers used discounts but spent above average
3	Top 5 Products by Rating	Gloves (3.86) · Sandals (3.84) · Boots (3.82)
4	Standard vs Express Shipping	Express avg: $60.48 · Standard avg: $58.46
5	Subscribers vs Non-Subscribers	Subscribers: 1,053 customers · Non-subscribers: 2,847
6	Most Discount-Dependent Products	Hat (50%) · Sneakers (49.66%) · Coat (49.07%)
7	Customer Segmentation	Loyal: 3,116 · Returning: 701 · New: 83
8	Top 3 Products per Category	Jewelry, Blouse, Sandals, Jacket top their categories
9	Repeat Buyers & Subscriptions	Most repeat buyers (2,518) are non-subscribers
10	Revenue by Age Group	Young Adult: $62,143 · Middle-aged: $59,197
---
📊 Power BI Dashboard
The interactive dashboard includes:
Visual	Description
🔢 KPI Cards	3.9K Customers · $59.76 Avg Purchase · 3.75 Avg Rating
🍩 Donut Chart	Subscription Status — Yes: 27% · No: 73%
📊 Bar Charts	Revenue & Sales by Category and Age Group
🎛️ Filters	Subscription Status, Gender, Category, Shipping Type
---
💡 Key Insights
🔹 Male customers generate more than double the revenue of female customers
🔹 Young Adults are the highest revenue-contributing age group ($62,143)
🔹 73% of customers are non-subscribers — a major opportunity for subscription growth
🔹 Loyal customers dominate — 3,116 out of 3,900 have made 10+ purchases
🔹 Express shipping users spend slightly more on average than standard shipping users
🔹 Hat, Sneakers, and Coat have the highest discount dependency (≈50%)
---
📋 Business Recommendations
Boost Subscriptions — Only 27% are subscribed; promote exclusive subscriber benefits to convert non-subscribers
Reward Loyal Customers — 3,116 loyal customers are the backbone; introduce a loyalty rewards program
Review Discount Policy — Products like Hat and Sneakers are heavily discount-dependent; balance discounts with margin control
Target Young Adults — They drive the highest revenue; focus marketing campaigns on this age group
Promote Top-Rated Products — Highlight Gloves, Sandals, and Boots in campaigns as they have the highest customer ratings
---
🛠️ Tools & Technologies
Tool	Purpose
Python (Pandas, Matplotlib, Seaborn)	Data cleaning & exploratory analysis
Jupyter Notebook	Interactive Python environment
PostgreSQL	Data storage & SQL business queries
Power BI	Interactive dashboard & data visualization
CSV	Raw data source
---
🚀 How to Run This Project
Step 1: Clone the Repository
```bash
git clone https://github.com/Nishant9034/customer-trends-analysis.git
cd customer-trends-analysis
```
Step 2: Run the Python Notebook
Open `Customer_Shopping_Behavior_Analysis.ipynb` in Jupyter Notebook
Run all cells to clean data and load it into PostgreSQL
Step 3: Run SQL Queries
Open `customer_behavior_sql_queries.sql` in pgAdmin or any SQL client
Execute queries to explore business insights
Step 4: Open Power BI Dashboard
Open `customer_behavior_dashboard.pbix` in Power BI Desktop
Connect to your PostgreSQL database if needed
---
📧 Feel free to connect with me on [LinkedIn](https://www.linkedin.com/in/nishant-kumar-786872292)
