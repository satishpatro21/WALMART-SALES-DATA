

# Walmart Sales Data Analysis

## Project Overview

This project aims to explore **Walmart Sales data** to identify top-performing branches and products, analyze sales trends across different categories, and understand customer behavior. The ultimate goal is to study how sales strategies can be optimized and improved based on data-driven insights.

The dataset was sourced from the **Kaggle Walmart Sales Forecasting Competition**, which provides historical sales data for 45 stores across various regions.

## Project Purpose

The major objective of this study is to gain deep insights into Walmart's sales operations and identify the key factors that influence the performance of different branches.

## Dataset Summary

The data contains **1,000 rows and 17 columns**, reflecting transactions from three distinct branches located in **Mandalay, Yangon, and Naypyitaw**.

| Column | Description | Data Type |
| --- | --- | --- |
| `invoice_id` | Unique ID for each sale | VARCHAR(30) |
| `branch` | Store branch (A, B, C) | VARCHAR(5) |
| `city` | Location of the branch | VARCHAR(30) |
| `customer_type` | Type of customer (Member/Normal) | VARCHAR(30) |
| `gender` | Gender of the customer | VARCHAR(10) |
| `product_line` | Category of the product | VARCHAR(100) |
| `unit_price` | Price per unit | DECIMAL(10, 2) |
| `quantity` | Number of units sold | INT |
| `VAT` | Value Added Tax (5%) | FLOAT(6, 4) |
| `total` | Total cost including tax | DECIMAL(10, 2) |
| `date` | Date of transaction | DATE |
| `time` | Time of transaction | TIMESTAMP |
| `payment_method` | Payment mode used | DECIMAL(10, 2) |
| `cogs` | Cost of Goods Sold | DECIMAL(10, 2) |
| `gross_margin_pct` | Gross margin percentage | FLOAT(11, 9) |
| `gross_income` | Gross Income | DECIMAL(10, 2) |
| `rating` | Customer satisfaction rating | FLOAT(2, 1) |

---

## Analysis Framework

### 1. Product Analysis

Analyzing different product lines to determine high-performers and those requiring marketing improvements.

### 2. Sales Analysis

Tracking sales trends to measure the effectiveness of applied business strategies and identifying necessary modifications to increase revenue.

### 3. Customer Analysis

Segmenting customers based on their behavior, purchasing trends, and individual profitability.

---

## Technical Roadmap

### **Phase 1: Data Wrangling**

* **Inspection:** Detecting NULL and missing values.
* **Database Design:** Creating a structured database and ensuring `NOT NULL` constraints are applied to maintain data integrity.

### **Phase 2: Feature Engineering**

Adding new descriptive columns to enhance the analysis:

* **`time_of_day`**: Categorizes sales into Morning, Afternoon, and Evening.
* **`day_name`**: Extracts the day (Mon, Tue, Wed...) to find the busiest periods.
* **`month_name`**: Extracts the month to determine peak seasonal performance.

### **Phase 3: Exploratory Data Analysis (EDA)**

Executing SQL queries and visualizations to answer core business questions regarding revenue, product popularity, and customer satisfaction.

---

## Business Questions to Answer

### **General & Product Insights**

* How many unique cities and branches are in the dataset?
* What is the most common payment method?
* Which product line generates the highest revenue and has the highest VAT?
* Which products are performing above average (Categorized as "Good/Bad")?

### **Sales & Customer Behavior**

* Which time of day sees the highest volume of sales per weekday?
* Which customer types (Member vs. Normal) contribute the most revenue?
* What is the gender distribution per branch?
* Which day of the week yields the best average customer ratings?
