---
title: "Core Concepts In Tableau"
datePublished: Wed Sep 17 2025 10:40:34 GMT+0000 (Coordinated Universal Time)
cuid: cmfnup9gq001102i2h14weulv
slug: core-concepts-in-tableau

---

## 📌 **Core Tableau Concepts**

### 1\. **Data Connection & Preparation**

* Connecting to different data sources (Excel, SQL, CSV, Cloud, etc.)
    
* Live vs Extract connections
    
* Joins, Unions, Blends
    
* Data types (string, number, date, boolean)
    
* Data roles (dimension vs measure)
    

---

### 2\. **Dimensions & Measures**

* **Dimensions (blue):** qualitative / categorical (e.g., Region, Category)
    
* **Measures (green):** quantitative / numerical (e.g., Sales, Profit)
    
* Aggregations (SUM, AVG, MIN, MAX, COUNT)
    

---

### 3\. **Discrete vs Continuous**

* **Discrete (blue pills):** categories → headers
    
* **Continuous (green pills):** ranges → axes
    
* Impacts how Tableau draws visuals
    

---

### 4\. **Marks & Shelves**

* Columns & Rows shelves (build the view)
    
* Marks card (color, size, label, detail, tooltip, shape)
    
* Pages shelf (animation / step-by-step filtering)
    

---

### 5\. **Filters**

* Dimension filters vs Measure filters
    
* Extract filters vs Data source filters vs Context filters
    
* Date filters (relative, range, starting, ending, special)
    
* "Only Relevant Values" filter option
    

---

### 6\. **Sorting & Grouping**

* Sort options: Axis, Field, Toolbar
    
* Grouping categories (manual groups, correcting inconsistencies)
    
* Sets (dynamic vs fixed subsets)
    

---

### 7\. **Hierarchies**

* Date hierarchy (Year → Quarter → Month → Day)
    
* Geographic hierarchy (Country → State → City → Postal Code)
    
* Custom hierarchies
    

---

### 8\. **Calculated Fields**

* Row-level calculations
    
* Aggregate calculations
    
* Table calculations (running total, percent of total, rank, moving average)
    
* Logical calculations (IF, CASE, IIF, ZN, ISNULL)
    

---

### 9\. **Visualization Types**

* Bar/line charts
    
* Maps (symbol, filled, density, path maps)
    
* Dual-axis & combo charts
    
* Scatter plots, bubble charts
    
* Histograms, boxplots, treemaps
    
* Highlight tables, heat maps
    

---

### 10\. **Dashboard & Story**

* Dashboards (combine multiple sheets, add interactivity)
    
* Actions (filter, highlight, URL actions)
    
* Stories (narrative-driven dashboards)
    

---

### 11\. **Performance & Optimization**

* Extracts vs live connections
    
* Context filters for performance
    
* Data source filters
    
* Minimizing custom SQL for speed
    

---

### 12\. **Order of Operations**

* Extract filters → Data source filters → Context filters → Dimension filters → Measure filters → Table calcs → etc.