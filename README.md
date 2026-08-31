# Power BI Customer Purchasing Behaviour Analysis

## Project Overview

### Introduction

This project analyses **customer purchasing behaviour using Microsoft Power BI**.

The main objective is to transform customer and purchase data into an interactive dashboard that helps users understand:

* Customer purchasing patterns
* Sales performance
* Product performance
* Customer segments
* Sales trends over time

The dashboard was designed to provide simple business insights that can support marketing, product and sales decisions.

---

## Dataset Information

The project uses two datasets:

### Customer Table

The Customer table contains customer information such as:

* Customer ID
* Gender
* Age
* Country
* Income

### Purchase Table

The Purchase table contains **50,000 purchase transactions** with information such as:

* Order ID
* Customer ID
* Product name
* Price
* Quantity
* Tax
* Shipping cost
* Order date
* Shipping date

The two tables are connected using `customer_id`.

---

## Project Objectives

The main objectives of this project are to:

* Analyse purchasing patterns by age, gender, country and income
* Identify products with the highest revenue and sales volume
* Analyse sales trends over time
* Identify important customer segments
* Provide simple business recommendations

---

## Data Preparation

Before creating the dashboard, the data was checked and prepared in Power BI.

The main steps included:

* Checking data types
* Checking date and numerical columns
* Checking missing values and duplicates
* Creating customer age groups
* Creating customer income groups
* Creating Year, Month Name and Month Number
* Sorting months into the correct calendar order

These steps helped prepare the data for analysis and visualisation.

---

## Data Model

A simple data model was created between the Customer and Purchase tables.

The relationship is:

`Customer[customer_id] 1 → * Purchase[customer_id]`

This means one customer can have multiple purchase transactions.

The relationship allows customer information such as age, gender, income and country to be used when analysing sales and purchasing behaviour.

---

## DAX Measures

Several DAX measures were created for the dashboard:

* **Total Revenue** – total sales revenue
* **Total Orders** – total number of orders
* **Total Customers** – number of customers
* **Average Order Value** – average spending per order
* **Total Shipping Cost** – total shipping cost

These measures automatically update when dashboard filters and slicers are used.

---

# Dashboard Analysis

The Power BI report contains four main dashboard areas.

## 1. Executive Dashboard

The Executive Dashboard provides a quick overview of business performance.

The main KPIs include:

* **Total Revenue: $351.15M**
* **Total Customers: 1K**
* **Total Orders: 50K**
* **Average Order Value: $7.02K**

The dashboard also includes:

* Total Revenue by Year
* Total Revenue by Country

This page provides a simple overview of overall sales performance.

---

## 2. Customer Analysis

The Customer Analysis dashboard explores purchasing behaviour across different customer groups.

The analysis includes:

* Customers by Gender
* Revenue by Income Group
* Revenue by Age Group
* Total Customers by Country

The dashboard helps identify customer groups that contribute more strongly to overall revenue.

One key observation is that the **High Income customer segment generates the highest revenue**.

---

## 3. Product Analysis

The Product Analysis dashboard compares product performance using:

* Top Products by Revenue
* Top Products by Quantity Sold

The dashboard also includes slicers for:

* Year
* Country
* Gender
* Age Group

One interesting finding is that **Curtains generated the highest total revenue**, while **Sports Shoes recorded the highest quantity sold**.

This shows that the product generating the most revenue is not always the product sold most frequently.

---

## 4. Sales Trend

The Sales Trend dashboard analyses purchasing activity over time.

The main charts include:

* Orders by Month
* Revenue by Month

These charts help identify changes in sales and purchasing activity throughout the year.

Interactive slicers allow the trends to be filtered by:

* Year
* Country
* Gender
* Age Group

---

# Key Findings

Some of the main findings from the dashboard include:

* High Income customers generate the highest revenue.
* Customer purchasing behaviour varies across age and income groups.
* Colombia has the highest revenue and the largest customer base.
* Curtains generate the highest product revenue.
* Sports Shoes have the highest quantity sold.
* Orders and revenue change across different months of the year.

These findings can help support customer targeting, product planning and sales decisions.

---

# Business Recommendations

Based on the dashboard analysis:

### Customer Targeting

Focus marketing and loyalty programmes on higher-value customer segments identified through the income and age analysis.

### Product Strategy

Maintain stock availability for high-performing products.

High-revenue products such as **Curtains** can be monitored for profitability, while high-volume products such as **Sports Shoes** can be supported through promotions and product bundles.

### Country Focus

Colombia is an important market because it has both the highest revenue and largest customer base.

The business can focus on retaining customers in Colombia while exploring growth opportunities in other countries.

### Sales Planning

Monthly sales trends can be used to support inventory, staffing and promotional planning.

---

## Project Files

The repository includes:

* **Power BI Dashboard (`.pbix`)** – interactive Power BI project
* **Project Report (`.docx`)** – explanation of the analysis and dashboard development
* **Project Presentation (`.pptx`)** – presentation of the project and findings
* **Data Dictionary (`.pdf`)** – description of the datasets, fields and measures

---

## Conclusion

The analysis covers customer demographics, product performance and sales trends. DAX measures and interactive slicers were used to allow users to explore the data from different perspectives.
