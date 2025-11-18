# 📘 Project Log — Power BI Superstore Sales Insights

This document tracks the day-by-day progress of the **Retail Sales & Profit Insights — Power BI Dashboard** project.  
The goal is to show clear, structured development — useful for recruiters, portfolio transparency, and personal learning.

---

## Day 1 — Data Preparation & Setup (Completed)

### ✔ Project Setup
- Created full project folder structure:
  - `/data`
  - `/pbix`
  - `/assets`
  - `/docs`
- Added the **Superstore CSV dataset** to `/data`
- Created Power BI file: `Superstore_Dashboard.pbix`

### Power Query Data Cleaning
- Loaded dataset into Power Query
- Corrected all data types
- Parsed dates using **Locale: English (United States)**  
  (Dataset uses `MM.DD.YYYY` with dots)
- Set `Postal Code` to **Text** (prevented leading-zero losses)
- Ensured numeric fields (`Sales`, `Profit`, `Discount`) use **Decimal Number**
- Standardized all column names (PascalCase)
- Performed error check (0 errors found)
- Marked redundant columns for later removal:
  - `Row ID`
  - `Country` (always “United States”)

### Status End of Day 1
Dataset is cleaned, validated, and prepared for dimensional modeling.

### Next Steps
- Build dimension tables:
  - Dim_Customer
  - Dim_Product
  - Dim_Geography
  - Dim_Date
- Create Fact table (Fact_Orders)
- Establish star schema relationships
- Add & configure Date Table for time intelligence

---

## Day 2 — Data Modeling (Planned)
- Create Date Table (Power BI or DAX)
- Define dimensions & fact table
- Set up 1:* relationships
- Mark Date Table
- Validate model with basic DAX measure (Total Sales)

---

## Day 3 — DAX Measures (Planned)
- Core metrics:
  - Total Sales
  - Total Profit
  - Profit Margin %
- Time intelligence:
  - YoY Sales
  - MoM Sales
- Category ranking & Top-N measures

---

## Day 4 — Dashboard Development (Planned)
- Layout setup (Executive Overview)
- Add visuals:
  - KPI cards
  - Trend lines
  - Category breakdown
  - Product performance
- Apply consistent theme & formatting

---

## Day 5 — Finalization (Planned)
- Polish visuals
- Add bookmarks/navigation (optional)
- Export images for GitHub
- Update README.md
- Record project summary

---

# Project Status
**Day 1 completed.**  
The dataset is fully cleaned and ready for modeling.
