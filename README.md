# Consumer Goods Domain Insights and Ad-hoc Queries

## Table of Contents
- [Project Overview](#project-overview)
- [Problem Statement](#problem-statement)
- [Task](#task)
- [Tools Used](#tools-used)
- [Quick Introduction](#quick-introduction)
  - Product
  - Customer
  - Region & Market
  - Fiscal Year
  - Data Model
- [Ad-hoc Requests](#ad-hoc-requests)

---

## Project Overview

This project focuses on providing business insights to management in the Consumer Goods domain using SQL and data visualization tools.

The analysis helps stakeholders understand:

- Product growth
- Customer trends
- Sales performance
- Market contribution
- Channel performance

The project simulates a real-world data analyst task where business stakeholders request insights based on company data.

---

## Problem Statement

AtliQ Hardware, a global computer hardware manufacturer, requires better data insights to support business decision-making.

To identify skilled data analysts, the company designed a SQL challenge to evaluate candidates' abilities in:

- SQL querying
- Data analysis
- Business insight generation
- Data visualization

Candidates analyze sales and financial datasets and present insights using:

- SQL queries
- Power BI dashboards
- Business reports

---

## Task

- Review the Ad-hoc business requests.
- Understand stakeholder requirements.
- Implement SQL queries to generate meaningful insights.
- Use visualization tools to present results clearly.
- Deliver insights suitable for top-level management.

---

## Tools Used

- MySQL
- Power BI
- PowerPoint

---

## Quick Introduction

### AtliQ Hardware

AtliQ Hardware is a computer hardware and peripherals manufacturer operating globally through multiple sales channels.

---

### Product

The `dim_product` table contains product-related data.

Products are structured as:

```
Division → Segment → Category → Product → Variant
```

![Products](https://github.com/Rajabhin/Consumer-Goods-Insights-and-Adhoc-queries/blob/main/Products.png)

---

### Customer

The `dim_customer` table contains customer-related information.

AtliQ serves customers through two platforms:

- Brick & Mortar
- E-Commerce

Products are sold through the following channels:

- Retailer
- Direct
- Distributor

![Customer Platform](https://github.com/Rajabhin/Consumer-Goods-Insights-and-Adhoc-queries/blob/main/Platform.png)

---

### Region / Market

Customers are grouped into four regions:

- APAC
- EU
- NA
- LATAM

The company operates in multiple countries within these regions.

![Region Market](https://github.com/Rajabhin/Consumer-Goods-Insights-and-Adhoc-queries/blob/main/Region_Market.png)

---

### Fiscal Year

The dataset follows a custom fiscal year structure.

![Fiscal Year](https://github.com/Rajabhin/Consumer-Goods-Insights-and-Adhoc-queries/blob/main/Fiscal_Year.png)

---

### Data Model

The following data model represents relationships between fact and dimension tables used for analysis.

![Data Model](https://github.com/Rajabhin/Consumer-Goods-Insights-and-Adhoc-queries/blob/main/Data_Model.png)

---

## Ad-hoc Requests

### 1
Provide the list of markets where customer **"Atliq Exclusive"** operates in the **APAC region**.

---

### 2
Calculate the **percentage increase in unique products in 2021 compared to 2020**.

Output fields:

- unique_products_2020
- unique_products_2021
- percentage_change

---

### 3
Generate a report showing **unique product counts for each segment**, sorted in descending order.

Output fields:

- segment
- product_count

---

### 4
Identify which segment had the **highest increase in unique products from 2020 to 2021**.

Output fields:

- segment
- product_count_2020
- product_count_2021
- difference

---

### 5
Retrieve the **products with the highest and lowest manufacturing costs**.

Output fields:

- product_code
- product
- manufacturing_cost

---

### 6
Generate a report showing the **top 5 customers with the highest average pre-invoice discount percentage in FY 2021 in the Indian market**.

Output fields:

- customer_code
- customer
- average_discount_percentage

---

### 7
Generate a **monthly gross sales report for the customer "Atliq Exclusive"**.

Output fields:

- Month
- Year
- Gross Sales Amount

This helps identify high-performing and low-performing months.

---

### 8
Identify which **quarter in 2020 recorded the highest total sold quantity**.

Output fields:

- Quarter
- total_sold_quantity

---

### 9
Identify the **sales channel contributing the highest gross sales in FY 2021** and its percentage contribution.

Output fields:

- channel
- gross_sales_mln
- percentage

---

### 10
Retrieve the **Top 3 products in each division with the highest total sold quantity in FY 2021**.

Output fields:

- division
- product_code
- total_sold_quantity
