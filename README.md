# 📊 Power BI Sales Project

This project is a full **Power BI end-to-end workflow** built with the Market dataset, a multi-national grocery chain with operations in Canada, Mexico, and the United States.  

It follows the complete **business intelligence process**:  
1. Connecting & shaping raw data  
2. Building a relational data model  
3. Adding calculated fields and DAX measures  
4. Designing an interactive report  

---

## 📂 Dataset
The project uses MavenMarket CSV files containing customer, product, store, region, calendar, transaction, and return data.  

Included resources:  
- `Maven_Market CSV Files.zip` — source datasets  
- `MavenMarket_Report.pbix` — Power BI file (project work)  
- `Maven_Market_Report_COMPLETE.zip` — reference solution  
- `Maven_Market.png` — project logo  

---

## 🔑 Project Workflow

### **Part 1: Connecting & Shaping the Data**
- Updated Power BI settings (disabled auto-relationships, set locale to English U.S.)  
- Connected and cleaned **Customers, Products, Stores, Regions, Calendar, Returns, Transactions** datasets  
- Fixed data types, promoted headers, and handled nulls  
- Created calculated columns such as:  
  - `full_name` (customer first + last name)  
  - `birth_year` (from birthdate)  
  - `discount_price` (90% of retail price)  
  - `full_address` and `area_code` (from store details)  
- Extracted calendar fields (start of week, month, quarter, year)  
- Combined 1997–1998 transactions into one fact table  

---

### **Part 2: Creating the Data Model**
- Organized tables in **star schema** with lookup tables above fact tables  
- Connected Transactions to Customers, Products, Stores, Calendar  
- Connected Returns to Products, Calendar, and Stores  
- Stores linked to Regions in a snowflake schema  
- Verified one-to-many relationships with proper filter direction  
- Formatted dates, currency, and geographic fields  

---

### **Part 3: Adding DAX Measures**
- Built calculated columns such as `Weekend`, `Current Age`, `Priority`, `Price_Tier`, etc.  
- Created measures for:  
  - Quantity Sold / Returned  
  - Total Transactions & Returns  
  - Return Rate %  
  - Weekend Transactions %  
  - Revenue, Cost, Profit, and Profit Margin  
  - YTD and 60-Day Revenue trends  
  - Revenue Targets (5% monthly lift)  
- Spot-checked results against reference totals  

---

### **Part 4: Building the Report**
- Designed a **Topline Performance** dashboard with:  
  - Matrix of transactions, profit, margin, and return rate by product brand  
  - KPI cards (transactions, profit, returns vs. last month)  
  - Map visual + country slicer for geographic analysis  
  - Treemap with drill-down (country → state → city)  
  - Column chart for weekly revenue trends (1998 filter)  
  - Gauge chart for revenue vs. target  
- Added bookmarks, notes, and interactive drill-through insights (e.g., Portland 1000 sales)  
- Applied conditional formatting, filters, and user-friendly visuals  

---

## 🎯 Purpose
The project demonstrates practical Power BI skills across the **entire BI pipeline** — from raw data to actionable insights.  

It serves as hands-on practice for:  
- Data cleaning and shaping in Power Query  
- Data modeling and schema design  
- DAX calculations and KPIs  
- Dashboard design and storytelling  

---

## 📷 Screenshots
*(Add screenshots of your report pages and data model here for visual documentation)*  

---

## 🚀 Next Steps
- Extend report with customer segmentation analysis  
- Add profitability KPIs at store and regional level  
- Explore Power BI advanced visuals (decomposition tree, smart narratives, key influencers)  

---

## 🛠 Tools Used
- Power BI Desktop  
- Power Query (ETL)  
- DAX (Data Analysis Expressions)  
- MavenMarket Dataset  

---
