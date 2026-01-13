#🛒 Walmart Sales Data Analysis & Optimization


#📌 Project Overview
This project involves a deep dive into Walmart Sales data to uncover the underlying patterns that drive retail success. By analyzing high-performing branches and products, we explore how variables like customer demographics, time of day, and product lines influence overall revenue.

The primary goal is to provide actionable insights to optimize sales strategies and improve customer engagement based on historical transaction data from the Kaggle Walmart Sales Forecasting Competition.

#📊 Data Insights & Structure
The dataset comprises 1,000 transactions across three prominent Walmart branches in Mandalay, Yangon, and Naypyitaw.

#Data Dictionary

Column	Description	Data Type
invoice_id	Unique identification for each sale	VARCHAR(30)
branch	Store branch identifier (A, B, C)	VARCHAR(5)
city	Location of the branch	VARCHAR(30)
customer_type	Member vs. Normal	VARCHAR(30)
product_line	Category of product sold	VARCHAR(100)
total	Final transaction amount (including tax)	DECIMAL(10, 2)
cogs	Cost of Goods Sold	DECIMAL(10, 2)
rating	Customer satisfaction score	FLOAT(2, 1)
Note: The dataset includes 17 features covering temporal, geographical, and financial metrics.

#🛠 Project Roadmap
#1. Data Wrangling

Integrity Checks: Verified that all fields adhere to NOT NULL constraints to ensure a clean dataset.

Database Management: Created a structured SQL environment to house and query the transaction data efficiently.

#2. Feature Engineering

To extract deeper insights, three new categorical features were generated:

time_of_day: Categorized transactions into Morning, Afternoon, and Evening to identify peak shopping hours.

day_name: Extracted the day of the week (Mon, Tue, etc.) to determine the busiest days for each branch.

month_name: Extracted the month to observe seasonal performance and monthly profit trends.

#3. Exploratory Data Analysis (EDA)

Our analysis is divided into three critical pillars:

Product Intelligence: Identifying high-growth product lines vs. underperforming ones.

Sales Forecasting: Analyzing transaction trends to measure the ROI of current sales strategies.

Customer Profiling: Segmenting customers by type, gender, and profitability to personalize future marketing.

#💡 Key Business Questions Answered
The analysis provides data-driven answers to questions such as:

Sales Performance: Which city generates the highest revenue? What is the total monthly revenue trend?

Inventory Optimization: What are the most common payment methods and the top-selling product lines?

Customer Behavior: Which customer segment (Member vs. Normal) contributes most to the VAT and total gross income?

Quality Control: Which product lines consistently receive the highest ratings from customers?

#🔢 Financial Formulas Used
The project utilizes specific financial metrics to calculate profitability:

Cost of Goods Sold:

COGS=unit_price×quantity
Value Added Tax:

VAT=5%×COGS
Total Revenue:

Total=VAT+COGS
Gross Profit:

Gross Income=Total−COGS
Gross Margin Percentage:

Gross Margin= 
Total Revenue
Gross Income
​
