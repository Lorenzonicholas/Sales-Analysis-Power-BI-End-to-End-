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
        

# Grouping

## Group

* **Select the members to group**
    
    * Click the **Paper** bar (or its axis label).
        
    * **Ctrl/⌘-click** the **Labels** bar so **both** are highlighted (you’ll see “2 items selected” in the tooltip).
        
* **Group from the selection**
    
    * On the small pop-up next to the selection, open the **caret/three-dot menu** and click **➕ Group Members**  
        *(or just right-click one of the selected bars →* ***Group****; or click the* ***paperclip*** *icon if it appears).*
        

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1757775271817/7de71443-86bd-44a5-bfe0-e21ca7905f15.png align="center")

## SET

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1757818791630/cf075211-4f11-4916-9321-a1ea14aeeb93.png align="center")

### Customised SET

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1757820661701/c583e26c-fe17-43b9-9f07-15a7c5a901df.png align="center")

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1757820709190/c43879fb-590e-4ec9-ae92-603f13145164.png align="center")

### Separate Color for SET

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1757820564592/32092378-a430-4032-b29e-5db9997564b1.png align="center")

### Filter with SET

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1757820470946/6a49a023-6417-4dc2-bc22-b81a7bc5d08a.png align="center")