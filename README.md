# Retail Sales & Profit Insights — Power BI Dashboard

## Overview
This project is a complete end-to-end Power BI solution built using the popular **Superstore** retail dataset.  
It demonstrates data cleaning, dimensional modeling, DAX calculations, time intelligence, and professional data visualization.

The final dashboard provides insights into:
- Revenue & Profit trends  
- Category & Product performance  
- Customer segments  
- Regional breakdown  
- YoY & MoM growth  

---

## 1. Data Preparation (Power Query)
Key cleaning steps:
- Corrected data types  
- Parsed dates using the correct locale  
- Standardized column names (PascalCase)  
- Removed potential data errors  
- Prepared structure for star schema  

---

## 2. Data Modeling
- Fact table: **Fact_Orders**  
- Dimensions: **Dim_Customer**, **Dim_Product**, **Dim_Geography**, **Dim_Date**  
- 1:* relationships  
- Marked Date table for proper time intelligence  

---

## 3. DAX Measures
Core business measures:
- `Total Sales`
- `Total Profit`
- `Profit Margin %`
- `YoY Sales`
- `MoM Sales`
- `Top Categories`
- `Top Products`

---

## 4. Dashboard Pages
- **Executive Overview**
- **Product Performance**
- **Customer Segments**
- **Trends & Time Intelligence**

---

## Folder Structure
/data -> dataset files
/pbix -> Power BI file(s)
/docs -> documentation, logs
/assets -> exported dashboard images


---

## 📝 Project Log
See `docs/project-log.md` for day-by-day progress.

---

## 🚀 How to Use
1. Download the `.pbix` file from the `/pbix` folder  
2. Open in **Power BI Desktop**  
3. Refresh the dataset (Superstore CSV included)

---

## 📌 Status
**Day 1 completed: Data cleaning finished. Modeling begins next.**
