# Retail Sales & Profit Insights — Power BI Dashboard
![Power BI](https://img.shields.io/badge/Power%20BI-Data%20Analytics-F2C811?style=flat&logo=powerbi&logoColor=black)

**Repository:** `powerbi-superstore-sales-insights`  
**Author:** Kuba Schwartz  
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

### ✔ Completed Cleaning Steps:

- Corrected all data types  
- Parsed date fields using **Locale: English (United States)**  
- Standardized column naming to PascalCase  
- Ensured Postal Code is stored as **text**  
- Checked dataset for row-level errors (none found)  
- Marked redundant columns for later removal  
  - Row ID  
  - Country (always "United States")

### 🧠 Important Notes:
- The Superstore CSV used here stores dates in **MM.DD.YYYY** format with dots  
- Sales & Profit must remain **Decimal Number**  
- Row ID is an artificial index and will not be used in the model

---

# 2. Data Model (Star Schema)

**To be completed in Day 2:**

- Fact_Orders  
- Dim_Customer  
- Dim_Product  
- Dim_Geography  
- Dim_Date

With the following relationships:

- Customer ID → Dim_Customer  
- Product ID → Dim_Product  
- Region/State/City → Dim_Geography  
- Order Date → Dim_Date  

A dedicated Date Table will be added and marked as the official Power BI date table for correct YTD / YoY / MoM calculations.

---

# 3. DAX Measures (Planned)

- `Total Sales`
- `Total Profit`
- `Profit Margin %`
- `YoY Sales`
- `MoM Sales`
- `Top Categories`
- `Top Products`
- `Profit by Segment`
- KPI Cards + Trend Lines

---

# 4. Dashboard Pages (Planned)

- **Executive Overview**
- **Product Performance**
- **Customer Segments**
- **Trends & Time Intelligence**

Each page will include clean visuals, consistent formatting, business storytelling, and navigation.

---

# Folder Structure
powerbi-superstore-sales-insights/
│
├── data/ # Superstore dataset (CSV)
├── pbix/ # Power BI dashboard file(s)
├── docs/ # Documentation, logs
├── assets/ # Exported dashboard images
└── README.md # Project documentation (this file)


---

# Project Log

## **Day 1 — Data Cleaning Completed**
- Created project folder structure  
- Added Superstore dataset (CSV)  
- Created Power BI file: `Superstore_Dashboard.pbix`  
- Loaded dataset into Power Query  
- Cleaned all fields, parsed dates, standardized names  
- Validated data & prepared for modeling  

**Next step:** Build dimensional model (Fact + Dimensions)

---

# How to Use

1. Download the `.pbix` file from the `/pbix` folder  
2. Open it in **Power BI Desktop**  
3. Refresh the data (dataset included under `/data`)  
4. Explore the dashboard or extend it with your own DAX measures

---

# Status

**Day 1 complete — Data cleaned & ready for modeling.**  
Day 2 will introduce relationships, a date table, and the first DAX measures.

---

