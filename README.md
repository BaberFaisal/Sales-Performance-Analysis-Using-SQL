# Sales Performance Analysis Using SQL

This project explores historical retail sales data to extract meaningful insights and optimize business strategies using SQL. The analysis includes customer behavior, product performance, branch-level trends, and profitability across various dimensions.

---

## Table of Contents

- [Project Overview](#project-overview)
- [Business Context](#business-context)
- [Analytical Strategy](#analytical-strategy)
- [Data Overview](#data-overview)
- [Advanced Data Cleaning](#advanced-data-cleaning)
- [Feature Engineering](#feature-engineering)
- [Business Metrics (KPIs)](#business-metrics-kpis)
- [Performance Analysis](#performance-analysis)
- [Customer Segmentation & Behavior](#customer-segmentation--behavior)
- [Product Line Analysis](#product-line-analysis)
- [Temporal Patterns](#temporal-patterns)
- [Payment Method Analysis](#payment-method-analysis)
- [Profitability Analysis](#profitability-analysis)
- [Correlations & Insights](#correlations--insights)

---

##  Project Overview

The project aims to support a retail chain in enhancing its sales strategy by analyzing transactional data using SQL. It focuses on performance metrics, customer segments, and profitability indicators.

---

## Business Context

A multi-branch retailer seeks to optimize:

- Inventory management  
- Promotional campaigns  
- Store operations  
- Customer engagement  

---

## Analytical Strategy

The approach includes:

- Cleaning and validating data  
- Feature engineering using time and customer attributes  
- KPI computation  
- Segmenting customers and products  
- Recommending improvements  

---

##  Data Overview

Key columns include:

- `Invoice ID`, `Branch`, `City`, `Customer type`, `Gender`, `Product line`  
- `Unit price`, `Quantity`, `Sales`, `Tax`, `COGS`, `Gross income`  
- `Date`, `Time`, `Payment`, `Rating`  

---

##  Advanced Data Cleaning

- Verified unique transactions  
- Checked for nulls and invalid entries  
- Standardized date/time formats  

---

## Feature Engineering

- Extracted day, month, hour, and time of day  
- Computed profit margins and weekend flags  

---

##  Business Metrics (KPIs)

- **Total Revenue:** `SUM(Sales)`  
- **Total Profit:** `SUM(Gross income)`  
- **Avg Basket Size:** `AVG(Quantity)`  
- **Avg Revenue per Transaction:** `AVG(Sales)`

---

## Performance Analysis

### Branch-wise & City-wise

| Branch | City       | Total Sales | Avg Rating | Total Profit |
|--------|------------|-------------|-------------|---------------|
| Giza   | Naypyitaw  | 110,568.79  | 7.03        | 5,265.18      |
| Alex   | Yangon     | 106,200.38  | 7.03        | 5,057.17      |
| Cairo  | Mandalay   | 106,197.68  | 6.82        | 5,057.03      |

---

##  Customer Segmentation & Behavior

- **By Type:** Members had higher average sales; Normals rated better  
- **By Gender:** Females spent more and bought more units  

---

##  Product Line Analysis

- **Top Revenue:** Food & Beverages, Sports & Travel  
- **Top Margin:** All lines had similar ~5% margin  

---

##  Temporal Patterns

- **Peak Sales Hour:** 8 AM  
- **Weekend vs Weekday:** Weekdays had more transactions  

---

##  Payment Method Analysis

| Payment   | Transactions | Total Sales | Avg Sale |
|-----------|--------------|-------------|----------|
| Cash      | 344          | 112,206.57  | 326.18   |
| Ewallet   | 345          | 109,933.11  | 318.82   |
| Credit    | 311          | 100,767.07  | 324.01   |

---

## Profitability Analysis

- **Most Profitable Branch:** Giza  
- **Consistent Margins:** All product lines maintained ~5% margin  

---

## Correlations & Insights

- High quantity + low rating may indicate overpromising products  
- Cash customers showed lower basket sizes  
- High-margin, low-volume products suggest premium pricing  

---

## Technologies Used

- SQL (MySQL/PostgreSQL syntax)
- Excel (data validation)
- PDF & Markdown reporting
