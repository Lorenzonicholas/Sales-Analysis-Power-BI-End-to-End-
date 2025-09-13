---
title: "Tableau Sorting / Grouping / Filtering"
datePublished: Sat Sep 13 2025 14:21:37 GMT+0000 (Coordinated Universal Time)
cuid: cmficu4y1000502jx0bx16pbq
slug: tableau-sorting-grouping-filtering

---

# Sorting

### Quick ways to sort in ascending and descending order

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1757773257993/c4762bea-1777-4d21-9410-9654f90fb9cc.png align="center")

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1757773579122/dfbbdc49-3d20-46eb-b3c1-fe5c19ca1da0.png align="center")

### Sort directly using the column value

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1757774062382/ba66f735-eca9-4775-a98f-56bd3ff8bbab.png align="center")

* **Data source order**
    
    * Keeps the members exactly in the order they come from the source (or the default order of the dimension).
        
    * Use when the source already has a meaningful sequence.
        
* **Alphabetic**
    
    * Sorts A→Z or Z→A by the **member names** (e.g., “Accessories”, “Appliances”…).
        
    * Ignores any measures on the view.
        
* **Field** ✅ *(most common for charts)*
    
    * Sorts the dimension by the **value of a field** (often a measure like **Sales**).
        
    * Choose the **Field** (e.g., *Sales*), the **Aggregation** (SUM/AVG/etc.), and **Ascending/Descending**.
        
    * Example: “Sub-Category sorted by **SUM(Sales)** descending” → bars ordered from biggest to smallest.
        
* **Manual**
    
    * Lets you **drag members** into any custom order (or use the **Manual** list in the dialog).
        
    * Great for business-defined sequences (e.g., “High, Medium, Low”).
        
* **Nested**
    
    * Used when you have **multiple dimensions** in the view.
        
    * Sorts **within each outer partition** instead of across the whole view.
        
    * Example: With **Region** then **Sub-Category**, a nested sort orders Sub-Categories by Sales **inside each Region** separately.