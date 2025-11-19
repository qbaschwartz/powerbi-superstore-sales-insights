# Project Log

## Day 1 — Data Cleaning Completed
- Created project folder structure  
- Imported Superstore CSV  
- Configured Power Query  
- Cleaned and validated all fields  
- Parsed date formats using correct locale  
- Standardized all column names  
- Prepared data for modeling

**Next step (Day 2):** Begin dimensional modeling

---

## Day 2 — Dimensional Model & First DAX Measures
- Built all dimension tables (Customer, Product, Geography, State, Date)  
- Prepared Fact_Orders table from the Superstore dataset  
- Established full Star Schema (1:* relationships, single-direction)  
- Organized Model View for clarity and documentation  
- Added initial core measures:  
  - Total Sales  
  - Total Profit  
  - Profit Margin %  
- Validated model and measures using test visuals (cards + slicers)  
- Ensured Date Table is marked as official Date Table for time intelligence

**Next step (Day 3):**  
Time Intelligence measures (YoY, MoM, Rolling 12M, YTD/MTD) and first dashboard visual layouts

---

# How to Use

1. Download the `.pbix` file from `/pbix`  
2. Open in **Power BI Desktop**  
3. Refresh data (CSV is included)  
4. Explore dashboard pages and measures  

---

# Status

**Day 2 complete — Dimensional model completed and core measures added.**  
Ready to proceed with Time Intelligence and dashboard visuals on Day 3.
