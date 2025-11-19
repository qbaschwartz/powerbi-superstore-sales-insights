# Retail Sales & Profit Insights — Power BI Dashboard
![Power BI](https://img.shields.io/badge/Power%20BI-Data%20Analytics-F2C811?style=flat&logo=powerbi&logoColor=black)

**Repository:** `powerbi-superstore-sales-insights`  
**Author:** Jakob Schwartz  
**Tools:** Power BI, Power Query, DAX, Data Modeling, CSV data

---

## Overview

This project is an end-to-end Power BI solution built using the popular **Superstore** retail dataset.  
It demonstrates professional skills in:

- Data cleaning (Power Query)
- Dimensional modeling (Star Schema)
- DAX calculations & time intelligence
- Dashboard design & data storytelling
- Business-focused insights

The dashboard focuses on **sales performance**, **profitability**, **category trends**, **customer segments**, and **regional breakdowns**.

---

# 1. Data Preparation (Power Query)

### ✔ Completed Cleaning Steps

- Corrected and validated all data types  
- Parsed date fields using **Locale: English (United States)**  
- Standardized column naming to PascalCase  
- Ensured Postal Code is stored as text  
- Removed unused or redundant columns  
  - Row ID (index only)  
  - Country (constant value)  
- Verified dataset contains no transformation errors

### Notes

- Original CSV uses dot-notation dates (e.g., `11.08.2016`)  
- Sales & Profit stored as decimal numeric fields  
- Data prepared for dimensional model design

---

# 2. Data Model (Star Schema)

The full dimensional model has been created and validated.

### Fact Table
- **Fact_Orders** (based on the Superstore dataset)

### Dimension Tables
- **Dim_Product**  
- **Dim_Customer**  
- **Dim_Geography**  
- **Dim_State** (added for proper hierarchical mapping)  
- **Dim_Date** (custom DAX-generated Date Table, marked as Date Table)

### Relationships (1:*)
- Fact_Orders → Dim_Product (Product ID)  
- Fact_Orders → Dim_Customer (Customer ID)  
- Fact_Orders → Dim_State (State)  
- Dim_State → Dim_Geography (hierarchical mapping)  
- Fact_Orders → Dim_Date (Order Date as active relationship)

All relationships are **single-directional** (Dimension → Fact) for clarity and performance.

---

# 3. DAX Measures

### Core Measures (Completed)
- `Total Sales`  
- `Total Profit`  
- `Profit Margin %`  

### Time Intelligence (Next)
- `YoY Sales`  
- `YoY Sales %`  
- `MoM Sales`  
- `Rolling 12M Sales`  
- `YTD Sales`  
- `MTD Sales`

### Planned Analytical Measures
- Top Categories  
- Top Products  
- Profit Contribution  
- Customer Ranking  
- KPI Cards and trend analysis sections  

---

# 4. Dashboard Pages (Planned)

- **Executive Overview**  
- **Product Performance**  
- **Customer Segments**  
- **Trends & Time Intelligence**  

Pages will include consistent formatting, clear storytelling, and a professional design layout.

---

# Folder Structure
powerbi-superstore-sales-insights/
│
├── data/ # Superstore dataset (CSV)
├── pbix/ # Power BI dashboard file(s)
├── docs/ # Documentation, logs
├── assets/ # Exported dashboard images
└── README.md # Project documentation


---

# Project Log

## Day 1 — Data Cleaning Completed
- Created project folder structure  
- Imported Superstore CSV  
- Configured Power Query  
- Cleaned and validated all fields  
- Parsed date formats  
- Prepared data for modeling

**Next step (Day 2):** Begin dimensional modeling

---

## Day 2 — Dimensional Model & First DAX Measures
- Built all dimension tables (Customer, Product, Geography, State, Date)  
- Prepared Fact table  
- Established full Star Schema (1:* relationships)  
- Organized Model View  
- Added initial DAX measures (Sales, Profit, Margin)  
- Verified model with test visuals (slicers + KPIs)

**Next step (Day 3):** Time Intelligence (YoY, MoM, Rolling 12M) + first dashboard visuals

---

# How to Use

1. Download the `.pbix` file from `/pbix`  
2. Open in **Power BI Desktop**  
3. Refresh data (CSV is included)  
4. Explore dashboard pages and measures  

---

# Status

**Day 2 complete — Dimensional model finished, core measures added.**  
Ready to proceed with Time Intelligence and visual design on Day 3.
