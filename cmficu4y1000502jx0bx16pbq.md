---
title: "Tableau Sorting / Grouping / Filtering"
datePublished: Sat Sep 13 2025 14:21:37 GMT+0000 (Coordinated Universal Time)
cuid: cmficu4y1000502jx0bx16pbq
slug: tableau-sorting-grouping-filtering

---

# Sorting

### Quick Ways to Sort in Ascending and Descending Order in Tableau

1. **Select the Chart**
    
    * Make sure your bar chart is active (for example, Sales by Sub-Category).
        
2. **Use the Sort Buttons on the Toolbar**
    
    * On the top toolbar, you’ll see two sort icons:
        
        * 🔼 **Ascending Sort** → sorts your bars from the smallest value to the largest.
            
        * 🔽 **Descending Sort** → sorts your bars from the largest value to the smallest.
            
    * Simply click one of these icons, and Tableau will reorder the bars accordingly.
        
3. **Click Directly on the Axis or Header**
    
    * Another quick way: hover near the axis label (like *Sub-Category*) or header in your chart.
        
    * A small sort icon will appear. Click it once for descending order, click again for ascending.
        

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1757773257993/c4762bea-1777-4d21-9410-9654f90fb9cc.png align="center")

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1757773579122/dfbbdc49-3d20-46eb-b3c1-fe5c19ca1da0.png align="center")

### Sorting Directly Using the Column Value in Tableau

1. **Right-Click on the Field (Dimension/Measure) in Columns or Rows**
    
    * In your chart, right-click on the field you want to sort (here it’s **Sub-Category** in the Columns shelf).
        
2. **Choose Sort…**
    
    * From the dropdown menu, click **Sort…** to open the sorting dialog box.
        
3. **Select the Sort By Option**
    
    * In the Sort dialog box, you’ll see multiple options under **Sort By**:
        
        * **Data Source Order** → Keeps the order as it appears in the dataset.
            
        * **Alphabetic** → Sorts items alphabetically (A → Z or Z → A).
            
        * **Field** → Sorts based on the values of another field (e.g., Sales, Profit).
            
        * **Manual** → Lets you drag and drop items in the exact order you want.
            
        * **Nested** → Sorts within the context of another dimension (useful for hierarchies).
            
4. **Choose Field Sorting**
    
    * Select **Field**, then pick which measure to sort by (e.g., **SUM(Sales)**).
        
    * Choose **Ascending** (lowest to highest) or **Descending** (highest to lowest).
        
5. **Click OK**
    
    * Tableau will immediately reorder your bars based on the chosen field values.
        

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1757774062382/ba66f735-eca9-4775-a98f-56bd3ff8bbab.png align="center")

# Grouping

### How to Create a Group in Tableau

1. **Locate the Field**
    
    * In the **Data pane**, right-click on the field you want to group.
        
    * In this example, you right-clicked on **Sub-Category**.
        
2. **Create Group**
    
    * From the menu, go to **Create → Group**.
        
    * A dialog box called **Create Group** will open.
        
3. **Select Items to Group**
    
    * In the dialog, select multiple members (e.g., *Labels*, *Paper*) that you want to combine.
        
    * Click the **Group** button.
        
    * Tableau will now treat them as a single grouped item (e.g., *Labels + Paper*).
        
4. **Finalize the Group**
    
    * You can rename the group if needed.
        
    * Check the option **Include “Other”** if you want Tableau to automatically create an “Other” category for ungrouped members.
        
    * Click **OK** to save.
        

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1757831024951/53d2d4b9-4e6e-47d8-b67c-4ddbf4ea5b1e.png align="center")

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1757830973175/2ff197ee-6277-42ff-a4ab-d8e90d252fe5.png align="center")

## SET

**How to Create a Set from the Top 10 Customers in Tableau**

1. In the view, **manually select the top 10 customer names** (by clicking and dragging over the bars, or using Ctrl + click).
    
2. Once the top 10 are highlighted, **hover over the selection menu** (the small drop-down icon on the tooltip bar).
    
3. From the menu, click **Create Set**.
    

You can now use this set in other charts to compare these top customers against the rest (e.g., Top 10 vs All Others).

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1757818791630/cf075211-4f11-4916-9321-a1ea14aeeb93.png align="center")

### Customised SET

**How to Create a Customized Set in Tableau (Top 10 Customers Example)**

1. **Right-click on the field you want to use for the set.**
    
    * In your case, you right-clicked on **Customer Name**.
        
2. **Go to → Create → Set.**
    
    * From the dropdown, select **Set…**.
        
    * This opens the **Create Set window**.
        
3. **Customize the Set.**
    
    * In the set dialog box, you can define rules:
        
        * **General tab** → Manually pick specific customers to include/exclude.
            
        * **Condition tab** → Apply conditions (e.g., include customers with Sales &gt; 50,000).
            
        * **Top tab** → Dynamically choose Top/Bottom *N* customers (like Top 10 by Sales).
            
    * In your case, you selected **Top 10 by Sales (SUM)**.
        
4. **Click OK** to create the set.
    
    * The new set will appear under the **Sets** section in the Data Pane.
        
    * You can then drag it into the view for analysis.
        

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1757820661701/c583e26c-fe17-43b9-9f07-15a7c5a901df.png align="center")

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1757820709190/c43879fb-590e-4ec9-ae92-603f13145164.png align="center")

### Separate Color for SET

**How to Apply Separate Colors for a Set in Tableau**

1. **Drag the Set to the Marks Card**
    
    * You already created a set (for example: **Top 10 Customers by Sales**).
        
    * Drag this set field onto the **Color** shelf in the **Marks card** (as shown in your screenshot).
        
2. **Tableau Automatically Splits the Data**
    
    * Tableau will color-code based on the set:
        
        * **IN** → Members inside the set (e.g., Top 10 Customers).
            
        * **OUT** → Members outside the set (all others).
            
3. **Customize the Colors**
    
    * Click on the **Color legend**.
        
    * Assign one color for **IN** (e.g., blue) and another for **OUT** (e.g., gray).
        
    * This makes it easy to visually distinguish the focus group (Top 10) from the rest.
        

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1757820564592/32092378-a430-4032-b29e-5db9997564b1.png align="center")

### Filter with SET

**How to Use a Set as a Filter in Tableau**

1. **Create a Set**
    
    * First, you already created a set (example: **Top 10 Customers by Sales**).
        
2. **Drag the Set to the Filters Shelf**
    
    * Go to the **Data pane** (left side).
        
    * Find your created set (e.g., *Set – Top 10 All Time*).
        
    * Drag it onto the **Filters shelf** (as shown in your screenshot).
        
3. **What Happens**
    
    * Tableau filters the view to show only members **IN** the set (in this case, the Top 10 customers).
        
    * The chart now displays only those top customers, hiding all others.
        

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1757820470946/6a49a023-6417-4dc2-bc22-b81a7bc5d08a.png align="center")

### **Filtering What’s IN vs OUT of a Set in Tableau**

When you create a Set (like *Top 10 All Time*), Tableau allows you to filter your view to show:

* **IN the Set** → members that satisfy the Set condition (e.g., Top 10 Customers by Sales).
    
* **OUT of the Set** → all other members that don’t meet the condition.
    

---

### **Steps (as shown in your screenshot):**

1. Go to the **Filters shelf** where your Set (e.g., *Set – Top 10 All Time*) is placed.
    
2. Right-click on the Set and choose **Show In/Out of Set**.
    
3. A filter dialog appears (right side of your screenshot). Here, you can:
    
    * ✅ Check **In** → Only members inside the Set appear (Top 10).
        
    * ✅ Check **Out** → Only members outside the Set appear (all others).
        
    * ✅ Check both → Compare “In” vs “Out” in the same visualization.
        

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1757821083786/4da0d324-fdd8-4b93-961d-6556a7b33bcc.png align="center")

### **Showing the Set Filter for Easy Selection**

Instead of always editing the Set manually, you can make things easier by showing the filter directly on the right-hand side of the view.

### **Steps:**

1. Go to the **Filters shelf** where your Set (e.g., *Set – Top 10 All Time*) is located.
    
2. Right-click on the Set and choose **Show Filter**.
    
3. Tableau will display a filter card on the right side of your view (as shown in your screenshot).
    
    * ✅ You can now easily toggle between **In**, **Out**, or **All** without reopening the Set dialog box.
        

### **Why this is useful:**

* Makes it **user-friendly** when building dashboards.
    
* Lets end-users quickly decide whether to see only top performers (*In*), the rest (*Out*), or everyone (*All*).
    
* Saves time compared to editing the Set each time.
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1757821342682/808c5dd8-675c-4d3f-843c-6625a943fe8a.png align="center")

### Creating a hierarchy

**How to Create a Category → Sub-Category Hierarchy in Tableau**

1. In the **Data pane** on the left, locate the fields **Category** and **Sub-Category**.
    
2. **Click and drag** `Sub-Category` onto `Category`.
    
    * Tableau will prompt you to create a **new hierarchy**.
        
3. In the pop-up window, **enter a name** for the hierarchy (e.g., **Product**).
    
4. Click **OK**.
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1757828890311/fc28c6d7-879c-41ee-b6bf-47a20e4f3b03.png align="center")

**🔽 Drilling Down from Category to Sub-Category**

1. On your chart, look at the **Columns shelf** where you placed **Category** (and later grouped with Sub-Category).
    
2. Notice the small **“+” icon** next to *Category*.
    
3. Click the **“+”** to **drill down**:
    
    * First it shows the broader view (*Category* level: Furniture, Office Supplies, Technology).
        
    * When you press **“+”**, Tableau expands the hierarchy to show the **Sub-Category** level under each Category (e.g., Chairs, Tables, Bookcases under Furniture).
        

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1757832429695/cb9cfb6e-18c6-40f4-8331-b545d77c65f9.png align="center")

### 🧩 Tableau’s Order of Operations

The **Order of Operations** in Tableau defines the sequence in which filters, computations, and actions are applied. Understanding this is crucial because applying filters at different stages can completely change the result of your visualization.

Here’s the simplified order:

1. **Extract Filters** – Applied first, restricts the data extracted from the source.
    
2. **Data Source Filters** – Limit rows/columns before they reach Tableau.
    
3. **Context Filters** – Set the context for other filters (e.g., Top N, Fixed LOD).
    
4. **Dimension Filters** – Filter based on categories (e.g., Region, Product).
    
5. **Measure Filters** – Applied on aggregated measures (e.g., SUM(Sales) &gt; 1000).
    
6. **Table Calculation Filters** – Filters after table calcs are computed (e.g., running totals).
    

👉 **Why it matters**:

* Filters earlier in the order reduce the dataset more efficiently.
    
* Filters later (like Table Calc) only affect what’s already been computed and displayed.
    
* Misplacing filters can lead to unexpected results.
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1757833364929/21efbddb-86f8-461a-a59a-bc26a8240f30.png align="center")

### Data Source Filters

### 📌 How to Apply a Data Source Filter in Tableau

1. **Right-click the Data Source** (e.g., *Maven Supplies*) in the Data Pane.
    
2. Select **Edit Data Source Filters…** from the dropdown menu.
    
3. In the pop-up window, click **Add…**.
    
4. From the field list, choose the field you want to filter on (e.g., **Order Date (MDY)**).
    
5. In the filter options, select **Range of Dates → Years**.
    
6. Choose the years you want to include (e.g., ✅ 2017, ✅ 2018).
    
7. Click **OK** to apply the filter.
    

---

### 🔑 What this does:

* A **Data Source Filter** applies before any sheet-level filters.
    
* It reduces the dataset at the source level, so Tableau only loads the filtered records.
    
* This improves performance and ensures consistency across all worksheets using this data source.
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1757834947389/4872d62c-e880-494c-b133-ce7a57a9effc.png align="center")

### Filter Shelf

📌 How to Add and Show Worksheet Filters in Tableau

1. **Drag a field to the Filters shelf**
    
    * For example, drag `Category`, `Region`, `Segment`, `State`, or `City` into the **Filters** area.
        
    * This limits the data based on your chosen filter values.
        
2. **Right-click the Filter (e.g., Category) → Show Filter**
    
    * This makes the filter visible on the worksheet.
        
    * The filter will now appear on the **right-hand side of the view** (or in the Filters pane).
        
3. **Interactive Filtering**
    
    * Users can now check/uncheck boxes to show or hide values (e.g., Furniture, Office Supplies, Technology).
        
    * This makes your chart interactive and dynamic.
        

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1757843910661/9863478a-733f-427c-af3f-87f79768047c.png align="center")

### 📌 Excluding Data in Tableau

1. **Right-click on a mark (bar, point, etc.) → Select *Exclude***
    
    * For example, in the chart, you right-clicked on *Furniture → Bookcases* and selected **Exclude**.
        
    * Tableau immediately removes that category from the view.
        
2. **Automatic Filter Creation**
    
    * When you exclude an item, Tableau automatically adds a new filter called **Exclusions** in the **Filters shelf**.
        
    * This filter contains the values you excluded.
        
3. **Editing the Exclusion Filter**
    
    * Right-click the new **Exclusions filter → Edit Filter**.
        
    * You will see the list of all possible values, with excluded ones marked.
        
    * From here, you can adjust what is excluded or bring values back into the view.
        

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1757844198232/dcbe3fb9-06b3-48f7-a747-dc17baba36fb.png align="center")

### 📝 Dimension Filter Card Modes

Dimension filters in Tableau can be displayed in different **card modes** to control how users interact with them:

1. **Single Value (List)**
    
    * Displays as radio buttons.
        
    * Allows only one selection at a time.
        
    * Best for small lists.
        
2. **Single Value (Dropdown)**
    
    * Single select, but shown as a dropdown.
        
    * Saves space compared to list.
        
3. **Single Value (Slider)**
    
    * Displays a slider to choose one dimension value (used when values have order, like dates).
        
4. **Multiple Values (List)**
    
    * Checkboxes for multiple selections.
        
    * More space required, auto-updates when selection changes.
        
5. **Multiple Values (Dropdown)**
    
    * Same as list, but compact.
        
    * Apply button is recommended.
        
6. **Multiple Values (Custom List)**
    
    * Allows typing in values to filter.
        
    * Useful for long lists with search capability.
        
7. **Wildcard Match**
    
    * Filters values based on a text pattern (e.g., all items containing "phone").