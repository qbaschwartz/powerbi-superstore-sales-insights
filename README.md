# Retail Sales & Profit Insights — Power BI Dashboard
![Power BI](https://img.shields.io/badge/Power%20BI-Data%20Analytics-F2C811?style=flat&logo=powerbi&logoColor=black)

Repository: `powerbi-superstore-sales-insights`  
Author: Jakob Schwartz  
Tools: Power BI, Power Query, DAX, Star Schema, Time Intelligence

---

## 1. Overview

This project is an end-to-end Power BI solution built on the popular **Superstore** retail dataset.  
It demonstrates:

- Professional data cleaning in Power Query  
- A clean **Star Schema** dimensional model  
- Custom DAX measures including **Time Intelligence**  
- KPI card design, trend visuals, and slicers  
- Business-focused insights for sales & profit performance  

The dashboard highlights trends in **Total Sales**, **Profit**, **Margin**, **YoY changes**, and **Rolling 12-Month performance**.

---

## 2. Data Preparation (Completed)

Data cleaning steps included:

- Corrected all data types  
- Parsed US-format dates using Locale EN-US  
- Standardized naming convention (PascalCase)  
- Ensured Postal Code stored as text  
- Removed redundant fields (e.g., Row ID, Country)  
- Validated dataset for errors (none remaining)

---

## 3. Data Model (Star Schema)

The following dimension tables were created:

- **Dim_Customer**  
- **Dim_Product**  
- **Dim_Geography**  
- **Dim_State**  
- **Dim_Date**

Main fact table:

- **Fact_Orders**

Relationships:

- Customer ID → Dim_Customer  
- Product ID → Dim_Product  
- State → Dim_State  
- City/Region → Dim_Geography  
- Order Date → Dim_Date  

Dim_Date was marked as the official date table for accurate Time Intelligence.

---

## 4. DAX Measures (Completed so far)

- Total Sales  
- Total Profit  
- Profit Margin %  
- Sales YTD  
- Sales MTD  
- Sales YoY  
- Sales YoY %  
- Sales Rolling 12M  
- Profit Rolling 12M  
- Profit YoY  

More analytical measures will be added on upcoming dashboard pages.

---

## 5. Dashboard Pages (In Progress)

### Page 1 — Executive Overview
Includes:

- KPI cards (Sales, Profit, Margin, YoY %, YTD, MTD)  
- Sales over Time (Total Sales + Rolling 12M)  
- Profit over Time (Total Profit + Rolling 12M)  
- Slicers: Date, Year, Category, State  

Next:  
- Page layout refinement  
- Additional trend visuals  
- Exporting assets for GitHub preview

---

## 6. Folder Structure
powerbi-superstore-sales-insights/
│
├── data/ # Superstore dataset (CSV)
├── pbix/ # Power BI dashboard
├── docs/ # Documentation & logs
├── assets/ # Exported dashboard images
└── README.md # Project documentation

---

## Status

**Day 3 in progress — Time Intelligence completed, Trend visuals added.**  
Next step: finish formatting, finalize Page 1 layout, export visuals for GitHub.

