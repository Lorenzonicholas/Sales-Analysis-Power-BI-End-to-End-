# Sales Analysis — Power BI (End-to-End)

**Introduction:**
- Built a star-schema model over multi-country retail data.
- Delivered exec-ready KPIs (MoM Transactions/Profit/Returns), geo insights, and product mix quality (Revenue vs Profit Share Gap).
- Focus on performance (single-direction filters, minimized M2M, measure catalog) and storytelling.

## Demo
### Topline Performance Interface
<img width="1767" height="961" alt="image" src="https://github.com/user-attachments/assets/d96478b4-cbdf-45ff-9011-d586a27a8766" />

### Products Interface
<img width="1755" height="1004" alt="image" src="https://github.com/user-attachments/assets/1bb97413-33c9-430b-953f-b79edd715d44" />


## What this project shows
- **Data Modeling:** clean star schema; fact tables filtered by shared dimensions; inactive/active relationships where needed.
- **Power Query:** type enforcement, locale control, merging & calculated columns (documented in `/powerquery`).
- **DAX:** YTD, MTD, rolling 60-day, prior-month comps, KPI targets, mix-gap metric. Full catalog in `/dax/measures.md`.
- **Executive Storytelling:** KPI cards, map + treemap drill, weekly trending, Top-20 profit brands, “Revenue vs Profit Share Gap.”

## Reproduce locally
1. Install Power BI Desktop (latest).
2. Clone this repo.
3. Open `pbix/Sales_Analysis.pbix`.  
   (If using sample data, switch to `/data_sample/` files via **Transform data → Data source settings**.)
4. Refresh.

## Data & License
- Data is sample/sanitized for demo; no PII.  
- License: MIT (see `LICENSE`).

## Contact
- LinkedIn: <your profile> • Email: <Lorenzo.nickolas@gmail.com>
