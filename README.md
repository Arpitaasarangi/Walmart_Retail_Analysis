# Walmart_Retail_Analysis

## 🎯 Objective
To uncover actionable business insights from Walmart’s retail transaction data using SQL and Power BI. The project focuses on customer behavior, branch performance, category profitability, and operational optimization. Each insight is tied to a real-world business decision—whether it's staffing, marketing, or inventory planning.

## 📂 Dataset Overview

- Source: Kaggle Walmart Sales Dataset
- Format: CSV
- Key Columns: Branch, City, Category, Payment_Method, Unit_Price, Quantity, Profit_Margin, Rating, Date, Time
The dataset captures transactional-level details including product category, customer ratings, payment method, and timestamped sales data across multiple Walmart branches.

## 🧰 Tools Used

- SQL (MySQL) – for structured querying and business logic
- Python (Pandas) – for data cleaning and preprocessing
- Power BI – for interactive dashboard visualization
- Excel – for initial data exploration and schema understanding

  
## 🧹 Data Cleaning Workflow

- Import Libraries
pandas, numpy, and datetime modules for data manipulation.
- Load Dataset
Read the CSV file and inspect the first few rows to understand structure.
- Check Shape & Descriptive Stats
Use .shape and .describe() to get a sense of volume and distribution.
- Handle Null Values
Use .isnull().sum() to detect missing data and drop or impute as needed.
- Remove Duplicates
Apply .drop_duplicates() to ensure clean transactional records.
- Data Type Conversion
- Convert unit_price to float for accurate calculations
- Parse date and time columns into a single datetime object
- Feature Engineering
Create a new column total = quantity × profit_margin to represent revenue contribution per transaction.
- Export Cleaned Data
Save the cleaned dataset to a new CSV file for SQL import.
- Load into MySQL
Establish connection and import the cleaned data into a relational database for querying.

## 🧠 Business Questions Solved (SQL Logic)

Each query was designed to answer a specific business challenge:
- Payment Preferences: What are the most used payment methods and how many items were sold through each?
- Branch Performance: Which branches generate the most revenue and which are declining year-over-year?
- Category Ratings: Which categories are most loved in each branch and city?
- Profitability: Which product categories yield the highest profit?
- Customer Behavior: What are the busiest days and shifts across branches?
- Regional Insights: Which cities have the highest average profit margins?
- Operational Planning: What is the most common payment method per branch?

## 📊 Power BI Dashboard Highlights
Your dashboard translates SQL insights into visual storytelling:
### KPIs: Total Revenue, Profit, Orders, Units Sold, Avg Rating
  
### Charts Used
- Bar chart for category performance
- Pie chart for payment method distribution
- Line chart for monthly sales trend
- Area chart for daily order volume
- Map for city-wise revenue distribution
- Bar chart for top 5 cities by revenue
Each visual is designed to support a business decision—whether it's marketing focus, staffing strategy, or payment system optimization.

## 🚀 How to Run

- Clone the repository git clone https://github.com/Arpitaasarangi/Walmart_Retail_Analysis.git
- Set up Python environment
- Install dependencies: pip install -r requirements.txt
- Run the Jupyter notebook
- Navigate to notebooks/EDA.ipynb
- Load cleaned data into MySQL
- Use sql/Walmart_queries.sql to import
- Execute SQL queries
- Open Power BI dashboard
- File: dashboard/Walmart_Dashboard.pbix

