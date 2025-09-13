---
title: "Microsoft Power BI Power Query Editor: A Complete Guide to Every Button and Icon"
seoTitle: "Microsoft Power BI Power Query Editor: A Complete Guide to Every Butto"
seoDescription: "Microsoft Power BI Power Query Editor: A Complete Guide to Every Button and Icon"
datePublished: Mon Aug 04 2025 09:14:00 GMT+0000 (Coordinated Universal Time)
cuid: cmdww8gec000g02l48li1g5bm
slug: microsoft-power-bi-power-query-editor

---

# Home Tab

The **Home tab** in Power Query Editor is your command center for data preparation. It brings together essential tools for loading, transforming, sorting, filtering, grouping, and combining data — all in one place. Whether you're starting a new query or applying the final touch before loading data into Power BI, this tab is where most of the action happens.

## 1 Close & Apply

When working with data in Power BI, the **Power Query Editor** acts as the central workspace for transforming and cleaning data before it’s loaded into the data model. But once your transformations are done, how do you finalize them?

That’s where the **“Close & Apply”** options come into play.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754399942987/f1cf39ff-a3a9-4f13-a3d5-129966282b3f.png align="center")

Let’s break it down:

### ✅ 1. **Close & Apply**

* Closes the Power Query Editor.
    
* Applies all the pending changes you’ve made.
    
* Loads the transformed data into Power BI’s data model for further analysis or visualization.
    

**👉 Use this when you’re done with all your transformations and ready to move back to the report view.**

### ✅ 2. **Apply**

* Applies the changes to the data model.
    
* Keeps the Power Query Editor open.
    

**👉 Ideal when you want to apply changes and continue working inside the Query Editor.**

### ✅ 3. **Close**

* Simply closes the Power Query Editor.
    
* **Does not apply** any changes made during the current session.
    

**⚠️ Warning:** You’ll lose all unsaved transformations if you select this.

### 💡 Best Practice Tip

Always **Apply or Close & Apply** your changes before exiting the Query Editor unless you're sure you don’t need those modifications. This avoids unintentional data loss.y understanding how these options work, you can better manage your data workflow and avoid accidental data loss or confusion while working in Power BI.

## 2 **New Source**

One of the most powerful features of Power BI is how easily you can bring in data from multiple sources—and it all starts from the **Power Query Editor**.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754400477866/5a620ba4-cd5d-411d-9ba1-a6b125797817.png align="center")

### 🧭 Navigation: Where to Find the “New Source” Option

Inside the **Power Query Editor**, go to the **Home** tab and locate the **New Source** button. Clicking this dropdown reveals several **most common data source options**, such as:

* 🟢 **Excel Workbook**
    
* 🟤 **SQL Server**
    
* 🟧 **Analysis Services**
    
* 📄 **Text/CSV**
    
* 🌐 **Web**
    
* 🔶 **OData Feed**
    
* 📃 **Blank Query**
    
* **More**
    

### **More Option**

### 🔍 The “Get Data” Window – A Closer Look

When you select **New Source &gt; More…**, it opens the **Get Data** window, where you’ll find an even broader range of connectors, grouped by category:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754400643307/30f2361c-1b79-4509-969d-03dd9c644522.png align="center")

| Category | Example Sources |
| --- | --- |
| **File** | Excel, Text/CSV, XML, JSON, PDF |
| **Database** | SQL Server, MySQL, Oracle, IBM Db2, Access |
| **Microsoft Fabric** | Data Warehouse, Lakehouse, KQL DB |
| **Power Platform** | Dataverse, Power BI datasets |
| **Azure** | Azure SQL, Blob, Data Lake, Synapse |
| **Online Services** | SharePoint, Salesforce, Dynamics 365 |
| **Other** | OData, Web, R/Script, Blank Query |

After selecting a data source, simply click **Connect**, then follow the authentication or path prompts to access your data.

### 💡 Pro Tip:

Use **Blank Query** when you want to manually write M code or fetch data via advanced scripts (e.g., calling APIs).

---

### 📌 Summary Table

| Feature | Description |
| --- | --- |
| New Source | Adds new data sources to your current Power BI project |
| Most Common List | Quick access to Excel, SQL, CSV, Web, and other top connectors |
| Get Data Window | Full list of categorized connectors (file, cloud, database) |
| Blank Query | Start from scratch or use M code for advanced queries |

Bringing in the right data is the **first step to powerful insights**, and Power BI makes that process seamless with a rich variety of connectors built right into the Power Query Editor.

## 3 Recent Sources

### 📂 Working with Recent Sources in Power BI (Power Query Editor)

Once you’ve connected to a data source in Power BI, you don’t have to go hunting for the file path every time you need to reuse it. Thanks to the **Recent Sources** feature, accessing your previously connected files is quick and effortless.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754400852008/c6530d82-43e6-4bcf-b7de-0d71a107c873.png align="left")

### What Does It Show?

When you click **Recent Sources**, a list labeled **Most Recent** appears—displaying the names of files or connections you’ve recently used.

Some examples from the screenshot:

* 📁 `Sample_Time_Functions_Table.csv`
    
* 📁 `Employee_Salary_StandardMath.csv`
    
* 📁 `Quarterly_Sales.csv`
    
* 📁 `JSON_files.csv`
    

These entries represent a wide variety of file formats: `.csv`, `.json`, `.xml`, and more.

### ⚙️ Why Is This Useful?

* **Speed**: Reconnect to recent files instantly without browsing through folders.
    
* **Consistency**: Reduces the chance of selecting the wrong file or version.
    
* **Workflow Efficiency**: Especially useful when switching between multiple datasets during report development.
    

## 4 Enter Data

### ✍️ Creating Tables Manually in Power BI: The “Enter Data” Option

Not all data comes from files or databases—sometimes, you just need to create a quick lookup table or manually enter a few values for testing. That’s where Power BI’s **Enter Data** feature comes in handy.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754401477147/3c99da5c-0c59-45cf-8d2f-ca8d45e2e2ec.png align="center")

### What Does “Enter Data” Do?

Clicking **Enter Data** opens a blank table editor window where you can manually:

* Add column headers
    
* Type in rows of data
    
* Rename the table
    

After you click **OK**, Power BI creates a new query with your manually entered data

### 💡 Pro Tip:

You can modify this table later just like any other query—add columns, merge it, apply filters, and more.

---

### 📌 Summary Table

| Feature | Description |
| --- | --- |
| Enter Data | Manually input data into Power BI as a new table |
| Use Cases | Lookup tables, filters, testing data |
| Editable Later | Yes – behaves like a regular query table |
| Location | Home tab → Power Query Editor |

---

Power BI is not just for connecting to external data—it also gives you the flexibility to create your own tables on the fly. Whether you need a quick fix or a functional supporting table, **Enter Data** is your go-to option.

## 5 Data Source Settings

### ⚙️ Managing Data Connections in Power BI: The “Data Source Settings” Window

In Power BI, working with multiple data sources is common. But what happens if a file path changes or you need to adjust permissions?

That’s where **Data Source Settings** comes in.

This powerful feature lets you manage, edit, and reset data connections—making your report both **dynamic** and **secure**.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754403979046/415cc8f6-7c41-4415-8540-16d47a540185.png align="left")

### 🗂️ What You’ll See

The **Data Source Settings** window displays a list of all sources you’ve connected to in the current report. You can choose between:

* **Data sources in current file** (default)
    
* **Global permissions** (across all Power BI files)
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754404065352/2067bb5b-9130-48b5-b448-eaabff934477.png align="left")

---

### 🛠️ Available Actions

At the bottom of the window, you’ll find a set of controls to manage these connections:

| Button | Function |
| --- | --- |
| **Change Source** | Update the file path, server, or location of the connected data |
| **Export PBIDS** | Export your connection info into a `.PBIDS` (Power BI Data Source) file |
| **Edit Permissions** | Modify authentication method (e.g., Anonymous, Windows, OAuth) |
| **Clear Permissions** | Reset credentials and remove stored authentication details |

---

### ✅ Use Cases

* 🔁 **Migrating projects** across environments or file locations
    
* 🔐 **Resetting access tokens or login methods**
    
* 🛡️ **Reviewing and managing data privacy levels**
    
* 🔗 **Fixing broken links** to local or cloud data sources
    

### 💡 Pro Tip:

If you're collaborating on a report, it’s good practice to **clear permissions** before sharing your `.pbix` file to avoid exposing sensitive login data.

## 6 Manage Parameters

### 🎛️ Dynamic Data Handling in Power BI: Using “Manage Parameters”

Parameters in Power BI are powerful tools that allow you to build dynamic, reusable, and flexible queries. Whether you want to filter data by date, file path, or region—you can create a parameter and reuse it across multiple queries.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754405576636/3120a628-0a64-4b5d-bf62-3aa17f5c86a7.png align="center")

### ➕ How to Create a Parameter

1. Click **New Parameter**
    
2. Give your parameter a **name** (e.g., `RegionFilter`)
    
3. Choose a **data type** (Text, Decimal Number, Whole Number, etc.)
    
4. Select the **Allowed Values** (List, Any value, or Query)
    
5. Define a **default value** and optionally a **current value**
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754405617215/0b94b66c-76ff-4840-88fe-6674f4fb1f35.png align="center")

Once created, the parameter will appear in the **Queries pane**, and you can reference it inside other queries.

---

### 🧪 Use Case Examples

* 📁 **Dynamic file paths**: Let users select different data sources
    
* 🌍 **Region filters**: Filter a query by region using a drop-down
    
* 📅 **Date filtering**: Only import rows after a given date
    
* ⚙️ **Query tuning**: Toggle between different modes or environments (e.g., dev/prod)
    

---

### 🔁 Reusability

The true power of parameters lies in **reuse**. Once defined, a parameter can be:

* Used in filters
    
* Referenced in M code
    
* Linked to dropdown slicers (via What-If parameters in Power BI Desktop)
    

---

### 📌 Summary Table

| Option | Purpose |
| --- | --- |
| **New Parameter** | Create a new dynamic input (number, text, etc.) |
| **Edit Parameters** | Modify existing parameters and values |
| **Use Cases** | File paths, filters, query switching, etc. |
| **Visibility** | Appears in Queries pane for reference |

## 7 Refresh Preview

### 🔄 Understanding "Refresh Preview" Options in Power BI

These options are found under the **Home** tab → **Refresh Preview** dropdown.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754407754608/3f537bbd-b670-4814-a13f-421ebb679b84.png align="center")

### 🔁 Available Options:

| Option | What It Does |
| --- | --- |
| **Refresh Preview** | Reloads data **only for the currently selected query**. Useful after parameter updates. |
| **Refresh All** | Refreshes **all queries** in the Power Query Editor. Good for full dependency updates. |
| **Cancel Refresh** | Stops an in-progress refresh. Useful if something is taking too long. |

---

### 🧪 When to Use It:

* After **editing a parameter value** (like `RegionFilter`)
    
* After **changing source files or filters**
    
* To **preview results** before applying changes with *Close & Apply*
    

## 8 Properties

### 🏷️ Rename and Document Your Queries: Using the “Properties” Option in Power BI

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754408137611/6885a5b2-a322-46c8-a4da-ff9c788fbb84.png align="center")

As your Power BI project grows, managing your queries effectively becomes essential. That's where the **Properties** option comes in—it helps you **rename** and **document** each query clearly.

### ✍️ What You Can Do with Properties

When you click **Properties**, a dialog box opens where you can:

| Field | Description |
| --- | --- |
| **Name** | Rename the query (e.g., from `Table1` to `sales_filter`) |
| **Description** | Add helpful notes for yourself or teammates |

### 💡 Why It Matters

* ✅ **Clean naming** helps during modeling and visualization
    
* 🧠 **Descriptions** act as mini-documentation
    
* 🤝 Useful for teamwork or handovers
    

### 🧪 Example Use Case:

| Before | After |
| --- | --- |
| Table1 | sales\_filter |
| Table2 | customer\_lookup |

### ✅ Pro Tip:

Use camelCase or snake\_case for consistency, especially if you’ll be referencing queries in M code or DAX. By using **Properties** to rename and document your queries, you build a cleaner, more maintainable Power BI project.

## 9 Advanced Editor

### 🧬 Writing and Editing M Code: Using the “Advanced Editor” in Power BI

Power BI gives you a rich graphical interface to transform data, but if you want **more control**, **automation**, or **custom logic**, the **Advanced Editor** is your go-to tool.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754408649084/26c2b67e-697f-4f80-8e9c-d1589bb21cff.png align="center")

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754409167333/34cfb1c5-b9a6-4ec8-87ad-49f543a8b0e1.png align="center")

### 🔍 What It Does

The **Advanced Editor** opens a window where you can view and edit the **M code** behind your query. This is the actual code Power BI generates every time you apply a transformation (like filter, rename, or merge).

### ✍️ When to Use It

* 🔁 To **copy/paste** query logic across files
    
* 🔍 To **understand or modify** step-by-step logic
    
* ⚙️ To **manually define** advanced steps (like dynamic filters, looping, or conditional logic)
    
* 🧪 To insert a **parameter** like `RegionFilter` in code
    

---

### 📌 Summary Table

| Feature | Description |
| --- | --- |
| Advanced Editor | Opens the M code behind your Power Query steps |
| Language | Power Query M Language |
| Use Cases | Custom logic, debugging, reuse, automation |
| Location | Home tab → Advanced Editor |

---

With **Advanced Editor**, you step beyond the GUI into the true engine room of Power BI—where everything becomes flexible and powerful.

## 10 Manage

### 🔁 Managing Queries in Power BI: Delete, Duplicate, and Reference

As you build and refine your Power BI project, you’ll often want to **reuse**, **branch**, or **clean up** queries. That’s where the **Manage** options — **Delete**, **Duplicate**, and **Reference** — come into play.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754409423809/218b6cf8-50e4-454a-bca6-d3840d372551.png align="center")

### 🧰 1. **Delete**

* ❌ Permanently removes the selected query.
    
* ⚠️ Warning: This cannot be undone inside Power Query Editor unless you cancel changes or revert.
    
* Useful for cleaning unused or test queries.
    

---

### 📄 2. **Duplicate**

* 📋 Creates a **copy** of the entire query.
    
* The duplicated query is **independent** of the original.
    
* Good when you want to create a slightly different version without altering the original.
    

**Example:**

> Duplicate `sales_table` → rename it `sales_last_month` and apply date filters separately.

---

### 🔗 3. **Reference**

* 🔁 Creates a **linked query** that **depends** on the original.
    
* It uses the original query as its **data source**, keeping the original untouched.
    
* Changes in the **base query** affect the reference query too.
    

**Example:**

> Create a reference of `all_sales` called `high_value_sales`, then filter it to only include orders &gt; $1000.

## 11 Choose Column

### 🧲 Focusing on the Right Data: Choose Columns in Power BI

When working with large tables in Power BI, you often don’t need every single column from the source. The **Choose Columns** tools help you quickly select or find the columns you care about — keeping your query lean and focused.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754409917231/2a57facd-6a63-4ca0-898f-510c0df687b3.png align="center")

### **Choose Columns option**

* Opens a checklist of all columns in your current query.
    
* You can **tick/untick** to include or remove columns.
    
* Very handy when you only need a few columns out of dozens.
    

**💡 Tip:** Hold `Ctrl` to select multiple columns quickly.

### **Go to Column option**

* Opens a searchable list of all columns.
    
* Helps you **jump directly to a specific column**, especially in wide tables.
    
* Doesn't remove columns — it just scrolls you into view.
    
    ### 🧪 Use Case Example
    

Imagine you’ve imported a wide table with 50+ columns, but you only need:

* `CustomerID`
    
* `OrderDate`
    
* `TotalAmount`
    

Use **Choose Columns** to quickly uncheck the rest and keep only the necessary fields.

### 📌 Summary Table

| Feature | Description | Action Type |
| --- | --- | --- |
| Choose Columns | Keep only selected columns from the dataset | Structural |
| Go to Column | Jump to a column by name, useful for navigation | Navigational |

## 12 Remove Columns

### 🧹 Clean Up Your Data: Using “Remove Columns” in Power BI Power Query

When you’re prepping data in Power BI, not all columns are useful. Some are redundant, others are just noise. The **Remove Columns** tool helps you quickly trim down your dataset.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754443673259/2c4936da-8fe9-4ef9-8e1d-4a2863c2221c.png align="center")

---

### ✂️ Two Main Options:

| Option | What It Does |
| --- | --- |
| **Remove Columns** | Deletes the **selected columns** only |
| **Remove Other Columns** | Deletes **everything EXCEPT** the columns you selected |

### 🧪 Use Case Examples

* 🗑️ Remove Columns: You imported a table with `FirstName`, `LastName`, `Email`, `SSN`, and you want to remove `SSN`.
    
* 🎯 Remove Other Columns: You only need `ProductID` and `SalesAmount` from a wide 40-column Excel sheet.
    

### ⚠️ Caution:

Removing columns **is irreversible** in the current query step unless you undo or delete the step manually.

* 🧼 **Undo Step**: In the **Applied Steps** pane, delete the **"Removed Columns"** step to restore all removed columns.
    
* 🧬 **Advanced Editor**: Edit the M code to remove or adjust the `Table.RemoveColumns` line.
    
* 🔁 **Go Back to Source**: Revisit an earlier step (like `Source`) and use **Choose Columns** to include the one you removed.
    

### 📌 Summary Table

| Feature | Description | Use Case |
| --- | --- | --- |
| Remove Columns | Deletes selected columns only | Hide/remove sensitive or unused fields |
| Remove Other Columns | Keeps selected ones, deletes the rest | Focus on specific key fields |

---

Use **Remove Columns** wisely to reduce noise, improve performance, and focus only on what your report truly needs.

## 13 Keep Rows

### 🔎 Focus on the Right Data: Using “Keep Rows” in Power BI

When you're working with raw data in Power BI, you often need to trim the dataset to focus only on specific parts — like keeping only the first 100 records, a certain range, or rows with duplicates. Power Query makes this easy with the **Keep Rows** tools.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754444124249/bf73e35d-47af-4787-86d0-29512f063893.png align="center")

### 🧰 1. **Keep Top Rows**

Keeps only the first *N* rows from the table.

✅ **Use it when**:

* You're sampling the first 100 records for a preview.
    
* Your data is sorted and you only need the latest entries (e.g., recent transactions).
    

### 🧰 2. **Keep Bottom Rows**

Keeps only the last *N* rows from the table.

✅ **Use it when**:

* You need to examine trailing data like recent logs or end-of-month entries.
    

### 🧰 3. **Keep Range of Rows**

Lets you keep a specific subset of rows starting from a chosen index.

✅ **Use it when**:

* You want rows from position 10 to 30.
    
* Useful for paginated analysis or testing a segment of your data.
    

### 🧰 4. **Keep Duplicates**

Keeps only the rows that have **duplicate values** in the selected column(s).

✅ **Use it when**:

* You’re identifying duplicate transactions, customer records, or IDs.
    
* Helpful in data quality checks and deduplication analysis.
    

### 🧰 5. **Keep Errors**

Keeps only the rows that contain **errors** (e.g., failed type conversions or missing values).

✅ **Use it when**:

* You’re auditing or debugging problematic data.
    
* You want to isolate and fix rows with issues.
    
    ### How to undo
    
* 🧼 **Undo the Step**: Go to the **Applied Steps** pane and delete the **"Kept Rows"** step — this will restore all rows.
    
* 🧑‍💻 **Advanced Editor**: Manually edit or remove the M code related to `Table.FirstN`, `Table.Range`, etc.
    

---

### 🧠 Tip:

Use **Keep Rows** carefully if you may need those rows again later — or create a **duplicate query** before filtering.

By mastering the **Keep Rows** options, you gain precise control over your data — helping you clean, validate, and optimize your dataset before building reports.

## 14 Remove Rows

### 🧹 Clean and Refine Data: Using “Remove Rows” in Power BI

Cleaning messy data is one of the most important steps in building accurate Power BI reports. The **Remove Rows** menu in Power Query gives you several powerful options to eliminate unnecessary or problematic rows from your dataset.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754444721956/4a0bd086-7ff3-4ad1-83b3-dcac7754fb26.png align="center")

### 🧰 1. **Remove Top Rows**

Removes a set number of rows from the **top** of the table.

✅ Use it when:

* Your file has header info or metadata in the top rows.
    
* You want to skip initial rows that aren’t actual data.
    

### 🧰 2. **Remove Bottom Rows**

Removes a set number of rows from the **bottom** of the table.

✅ Use it when:

* There are summary totals or footer notes in the last few rows.
    
* You want to exclude closing remarks from text exports.
    

### 🧰 3. **Remove Alternate Rows**

Removes every other row (or based on a pattern you define).

✅ Use it when:

* You're cleaning sensor logs, testing patterns, or skipping staggered data entries.
    
* Useful for sampling alternate entries in structured formats.
    

### 🧰 4. **Remove Duplicates**

Removes all **duplicate rows** based on selected column(s).

✅ Use it when:

* You want each entry (e.g., customer, invoice) to appear only once.
    
* Useful in cleansing repeated rows from Excel exports or merged tables.
    

### 🧰 5. **Remove Blank Rows**

Deletes rows where all columns are empty.

✅ Use it when:

* Cleaning imports with large blank gaps.
    
* Improving data compactness for modeling.
    

### 🧰 6. **Remove Errors**

Removes rows that contain **errors** in any column.

✅ Use it when:

* You want to ignore data conversion or formula issues.
    
* Great for skipping problematic records instead of fixing them (when acceptable).
    

### 📌 Summary Table

| Option | Purpose | When to Use It |
| --- | --- | --- |
| Remove Top Rows | Deletes rows from the top | Skip headers, intro lines |
| Remove Bottom Rows | Deletes rows from the end | Skip footnotes, summaries |
| Remove Alternate Rows | Deletes in a pattern (e.g., every 2nd) | Sampling, staggered data |
| Remove Duplicates | Deletes repeating rows | Ensure data uniqueness |
| Remove Blank Rows | Deletes empty rows | Clean up structure |
| Remove Errors | Deletes error-containing rows | Avoid loading broken records |

---

## 15 Sorting Data

### 🔃 Sorting Data in Power Query Editor – Power BI

Sorting is one of the simplest yet most effective data transformation tools in Power BI’s Power Query Editor. With just a click, you can reorder your data to make it easier to understand, analyze, and clean.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754451776116/285b56ca-e59c-46f7-95ea-6119e5a41841.png align="center")

### 🔼 Sort Ascending (A → Z)

This option sorts the selected column in **ascending order**:

* For text: A to Z
    
* For numbers: Smallest to largest
    
* For dates: Oldest to newest
    

### 🔽 Sort Descending (Z → A)

This option sorts the selected column in **descending order**:

* For text: Z to A
    
* For numbers: Largest to smallest
    
* For dates: Newest to oldest
    

Sorting may seem like a small step, but in Power Query, it sets the foundation for cleaner, more meaningful data transformations.

## **16 Split Column**

### ✂️ Splitting Columns in Power Query – A Smart Way to Reshape Your Data

When cleaning or preparing data in Power BI’s Power Query Editor, one common task is to break a single column into multiple parts. That’s where the **“Split Column”** tool comes in — a flexible and powerful feature under the **Home tab**.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754452021041/4b738dcc-e927-4721-8d02-6be9fe0a3620.png align="center")

### 1️⃣ **By Delimiter**

Splits the column wherever a specific character appears (e.g., comma, space, hyphen).  
📌 Example: `"John,Smith"` ➜ `John` | `Smith`

✅ Best for:

* Full names
    
* Addresses
    
* CSV-style data in one cell
    

### 2️⃣ **By Number of Characters**

Splits the column every *n* characters.  
📌 Example (every 3 characters): `"ABCDEF"` ➜ `ABC` | `DEF`

✅ Best for:

* Fixed-format codes (like account numbers)
    
* Batch IDs
    

### 3️⃣ **By Positions**

Splits the column at defined character positions.  
📌 Example (at positions 2 and 4): `"123456"` ➜ `12` | `34` | `56`

✅ Best for:

* Structured data strings
    
* Phone numbers or ID codes
    

### 4️⃣ **By Lowercase to Uppercase**

Splits when a lowercase letter is followed by an uppercase one.  
📌 Example: `"dataScience"` ➜ `data` | `Science`

✅ Best for:

* CamelCase or mixed-format words
    

### 5️⃣ **By Uppercase to Lowercase**

Splits when an uppercase letter is followed by a lowercase letter.  
📌 Example: `"JSONData"` ➜ `JSON` | `Data`

✅ Best for:

* Acronym + word combinations
    

### 6️⃣ **By Digit to Non-Digit**

Splits at the boundary where digits end and letters start.  
📌 Example: `"123ABC"` ➜ `123` | `ABC`

✅ Best for:

* Product codes (e.g., "456XTV")
    

### 7️⃣ **By Non-Digit to Digit**

Opposite of the above: splits where letters end and digits start.  
📌 Example: `"XYZ789"` ➜ `XYZ` | `789`

✅ Best for:

* Alphanumeric strings
    

---

## 🎯 Final Thoughts

The **Split Column** feature is more than just a basic tool — it's a data preparation essential. Whether you’re parsing names, breaking apart structured codes, or untangling mixed content, these split options offer a fast and customizable solution.

✏️ *Clean data = better reports. Use “Split Column” to make your tables smarter and more structured.*

## 17 Group By

### 📊 Power Query's “Group By” Feature – Summarize and Simplify Your Data

In Power BI’s Power Query Editor, the **Group By** tool is a powerful way to **aggregate and summarize** data. Whether you're analyzing sales by region, counts by category, or totals by date, this feature helps reduce large datasets into meaningful insights — before they even reach your report visuals.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754453943909/ac8a1312-f37b-4447-9701-ea90839c3339.png align="center")

### 🧩 What Does “Group By” Do?

The **Group By** function lets you:

* **Group rows** based on one or more columns
    
* **Aggregate values** using built-in operations like count, sum, average, min, max, etc.
    

This is similar to using `GROUP BY` in SQL or pivoting data in Excel.

### 📌 Example Scenario

You have this table:

| Region | Sales |
| --- | --- |
| East | 100 |
| West | 200 |
| East | 150 |

If you apply **Group By Region** with a **Sum of Sales**, you get:

| Region | Total Sales |
| --- | --- |
| East | 250 |
| West | 200 |

### ⚙️ Steps to Use "Group By" in Power Query

1. Select the column(s) you want to group by (e.g., Region)
    
2. Click **Group By** in the Home tab
    
3. In the popup:
    
    * Choose the column to group
        
    * Add an aggregation (e.g., sum, count, average)
        
4. Click OK
    

🎛️ You can also add multiple aggregations or group by more than one column using **Advanced** mode.

---

### 🛠️ Common Aggregation Types

| Operation | Description |
| --- | --- |
| Sum | Total of values |
| Count | Number of rows in each group |
| Average | Mean value |
| Min/Max | Smallest or largest value |
| All Rows | Keeps all rows in a nested table |

### 🧠 Pro Tips

* Use **Group By** early in your query steps to reduce data size
    
* Combine with **Sort** to control which records appear first
    
* Use **All Rows** when you want to apply custom logic after grouping
    

---

## ✅ Final Thoughts

The **Group By** tool is more than just a way to summarize — it’s a gateway to building efficient and clean data models. Whether you're counting customers, summing revenue, or isolating records by condition, mastering this feature gives you a major edge in Power BI data prep.

## 18 Data Type

### 🔠 Power BI Power Query: Understanding Data Types – Clean Data Starts Here

In Power BI’s Power Query Editor, one of the most fundamental steps in data preparation is assigning the correct **data type** to each column. Why? Because data types directly affect sorting, filtering, calculations, visualizations, and performance.

You can define data types using the **“Data Type” dropdown** (as highlighted in your screenshot). Let’s explore each option and when to use it.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754456310930/22da8ba0-d55e-4bd5-80d1-37ac8f485335.png align="center")

### 📊 List of Data Types in Power Query

| Data Type | Description |
| --- | --- |
| **Decimal Number** | Supports floating-point numbers (e.g., 99.99). Ideal for precise values. |
| **Fixed Decimal Number** | Stores numbers with fixed decimal places — useful for currency values. |
| **Whole Number** | For integers only (e.g., 1, 100, -25). |
| **Percentage** | Converts numbers like 0.75 into 75%. |
| **Date/Time** | Combines both date and time. Useful for timestamps. |
| **Date** | Stores only the calendar date (e.g., 2025-08-06). |
| **Time** | Stores only the time portion (e.g., 14:30:00). |
| **Date/Time/Timezone** | Includes timezone offset for global date tracking. |
| **Duration** | Represents time intervals (e.g., 5 days, 4 hours). |
| **Text** | For strings, like names, codes, and descriptions. |
| **True/False** | Boolean values: `true` or `false` only. |
| **Binary** | Stores binary files like images or documents — rarely used in simple ETL. |

### 🧪 Why Setting the Right Data Type Matters

* ✅ **Accurate calculations**: Dates calculate date differences; numbers compute sums.
    
* ✅ **Efficient sorting/filtering**: Numeric vs text sorting behaves differently.
    
* ✅ **Prevents errors**: Many Power BI functions rely on correct data types.
    
* ✅ **Better visuals**: Data types determine chart axes and aggregations.
    

## 💡 Pro Tips

* Always check data types right after importing data.
    
* Power BI often guesses types, but it’s not always correct — verify!
    
* Use **"Detect Data Type"** option for auto-assignment, but always double-check.
    

## **19 Use First Row as Headers**

### **📊 Power BI Desktop Study Note: Mastering the "Use First Row as Headers" Feature**

**🔍 Overview**

When working with raw data in Power BI Desktop, especially from sources like Excel or CSV files, it's common to encounter datasets where the first row contains column names rather than actual data. Power BI provides a simple yet powerful tool to handle this: **"Use First Row as Headers"**, found under the **Transform tab**.

![](data:image/png;base64,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 align="left")

**🛠️ What Does "Use First Row as Headers" Do?**

This feature **promotes the first row of your dataset to become the column headers**. It’s especially useful when:

* You import data and Power BI doesn’t automatically recognize the headers.
    
* Your dataset starts with descriptive labels like "Name", "Date", "Sales", etc., but they’re treated as data rows.
    

**✅ Example:**

Suppose your table looks like this:

| **Row** | **Column1** | **Column2** | **Column3** |
| --- | --- | --- | --- |
| 1 | Date | Sales | Region |
| 2 | 2025-01 | 1000 | West |

After clicking **"Use First Row as Headers"**, it becomes:

| **Date** | **Sales** | **Region** |
| --- | --- | --- |
| 2025-01 | 1000 | West |

**🔄 Bonus: "Use Headers as First Row"**

This adjacent option **demotes the current headers back into the first row**. It’s useful when:

* You want to temporarily treat headers as data.
    
* You’re restructuring or pivoting your dataset.
    

**🧠 Why It Matters**

Proper headers are crucial for:

* Accurate data modeling.
    
* Clear visualizations.
    
* Smooth transformations and filtering.
    

Using these options ensures your dataset is structured correctly before diving into deeper analysis.

**📝 Final Thoughts**

The **"Use First Row as Headers"** tool is a small but mighty feature in Power BI Desktop. It’s part of the essential data preparation toolkit that helps you turn messy imports into clean, analyzable tables. Whether you're a beginner or a seasoned analyst, mastering this feature will save you time and headaches.

## **20 Replace Values**

### **🔄 Power BI Study Note: Mastering the "Replace Values" Tool in the Transform Tab**

When working with real-world data, inconsistencies and unwanted values are inevitable. Whether it's typos, placeholder text, or outdated labels, cleaning your data is a crucial step before analysis. Power BI Desktop offers a powerful feature to help with this: **"Replace Values"**, located in the **Transform tab**.

![](data:image/png;base64,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 align="left")

**🛠️ What Does "Replace Values" Do?**

The "Replace Values" feature lets you:

* **Find and replace** specific entries in a column.
    
* Standardize inconsistent data.
    
* Remove unwanted placeholders or errors.
    

**✅ Example:**

Imagine a column with values like:

\["N/A", "Completed", "In Progress", "n/a", "Complete"\]

You can use "Replace Values" to:

* Replace "N/A" and "n/a" with "Not Available"
    
* Replace "Complete" with "Completed"
    

This ensures consistency and improves the quality of your analysis.

**💡 Pro Tips**

* Use **case-sensitive matching** carefully—Power BI treats "N/A" and "n/a" as different unless specified.
    
* Combine with **"Remove Rows"** or **"Filter"** for deeper cleaning.
    
* Use **"Replace Errors"** if you're dealing with error values instead of regular text.
    

**📝 Final Thoughts**

The **"Replace Values"** feature in Power BI Desktop is simple yet powerful. It empowers analysts to clean and standardize data efficiently, ensuring that downstream reports and dashboards are built on a solid foundation. Mastering this tool will save you time and elevate the quality of your insights.

## **21 Merge Queries**

### **🔗 Power BI Study Note: Demystifying the "Merge Queries" Feature**

In Power BI Desktop, combining data from multiple tables is a common and essential task. Whether you're working with sales data from different regions or customer information spread across systems, **"Merge Queries"** is your go-to tool for joining datasets efficiently.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754488299890/705cae6b-2f85-47f7-bfdd-2983da441f89.png align="center")

### **🔄 What Does "Merge Queries" Do?**

"Merge Queries" allows you to **join two tables based on a common column**, similar to SQL joins. You can choose the type of join (e.g., Left, Right, Inner, Full Outer) depending on your data needs.

#### **✅ Example:**

Suppose you have:

* A **Sales** table with `CustomerID`, `Date`, and `Amount`.
    
* A **Customers** table with `CustomerID`, `Name`, and `Region`.
    

Using "Merge Queries," you can join these tables on `CustomerID` to enrich your sales data with customer details.

### **🖼️ Visual Walkthrough: Merge Dialog Box**

The Merge dialog box in Power BI’s Power Query Editor allows you to:

* Select the tables and columns to merge.
    
* Choose from various **Join Kinds**:
    
    * **Left Outer**: All rows from the first table, matched rows from the second.
        
    * **Right Outer**: All rows from the second table, matched rows from the first.
        
    * **Full Outer**: All rows from both tables.
        
    * **Inner**: Only rows with matches in both tables.
        
    * **Left Anti**: Rows only in the first table.
        
    * **Right Anti**: Rows only in the second table.
        

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754489290871/b4b07f4c-463b-4ee6-989f-fa7a638674bf.png align="center")

### **🔍 Advanced Feature: Fuzzy Matching**

Sometimes, data entries don’t match exactly due to typos or formatting differences. Power BI offers **Fuzzy Matching** to help with this.

#### **Fuzzy Matching Options:**

* **Similarity Threshold**: Set a value (e.g., 0.80) to define how closely values must match.
    
* **Ignore Case**: Checked by default to treat "ABC" and "abc" as equal.
    

This is especially useful when merging datasets with inconsistent naming conventions or human-entered data.

### **📝 Final Thoughts**

The **"Merge Queries"** feature in Power BI Desktop is a powerful tool for data integration. Whether you're building dashboards or performing deep analysis, mastering this feature will help you create more meaningful and connected insights.

## 22 **Append Queries**

### **➕ Power BI Study Note: Understanding the "Append Queries" Feature**

In Power BI, data often comes from multiple sources or files that share the same structure—like monthly sales reports or regional customer lists. To analyze this data as a single dataset, you can use the **"Append Queries"** feature in Power BI Desktop.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754490084289/7cee514b-5772-43bf-ab8c-0c9f065b0f3b.png align="center")

### **🔄 What Does "Append Queries" Do?**

Appending queries means **stacking tables vertically**—adding rows from one table to another. This is different from merging, which joins tables side-by-side based on a key column.

#### **✅ Example:**

You have two tables:

**Sales\_January**

| **Date** | **Region** | **Sales** |
| --- | --- | --- |
| 2025-01-01 | North | 1000 |
| 2025-01-02 | South | 1200 |

**Sales\_February**

| **Date** | **Region** | **Sales** |
| --- | --- | --- |
| 2025-02-01 | North | 1100 |
| 2025-02-02 | South | 1300 |

Using **Append Queries**, you get:

**Combined\_Sales**

| **Date** | **Region** | **Sales** |
| --- | --- | --- |
| 2025-01-01 | North | 1000 |
| 2025-01-02 | South | 1200 |
| 2025-02-01 | North | 1100 |
| 2025-02-02 | South | 1300 |

### **🧠 Why It Matters**

Appending is ideal for:

* Combining data from multiple periods (e.g., monthly reports).
    
* Consolidating regional datasets.
    
* Preparing unified data for analysis and visualization.
    

It’s a clean and efficient way to build a comprehensive dataset without altering the original sources.

---

### **📝 Final Thoughts**

The **"Append Queries"** feature in Power BI is a powerful tool for data consolidation. Whether you're working with time-series data, departmental reports, or multi-source inputs, appending queries helps you streamline your workflow and prepare your data for meaningful insights.

## 23 **Combine Files**

### **📁 Power BI Study Note: Unlocking the Power of "Combine Files"**

When working with data from multiple files—especially those stored in folders—Power BI Desktop offers a powerful automation tool: **"Combine Files"**. This feature is a game-changer for analysts who regularly deal with structured data spread across multiple Excel sheets, CSVs, or text files.

In this study note, we’ll explore what **Combine Files** does, how to use it, and why it’s ideal for scalable, repeatable data preparation.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754490618464/3edb75e2-9ff9-4e7c-afcf-583429fe4214.png align="center")

### **📂 What Does "Combine Files" Do?**

**Combine Files** automates the process of:

* Reading multiple files from a folder.
    
* Applying a consistent transformation to each file.
    
* Stacking the results into a single, unified table.
    

It’s especially useful when all files share the same structure—like monthly reports or daily logs.

### **✅ Example Scenario**

Imagine you have a folder with these CSV files:

* `Sales_Jan.csv`
    
* `Sales_Feb.csv`
    
* `Sales_Mar.csv`
    

Each file contains:

| **Date** | **Region** | **Sales** |
| --- | --- | --- |
| 2025-01-01 | North | 1000 |
| 2025-01-02 | South | 1200 |

Using **Combine Files**, Power BI will:

1. Read all files in the folder.
    
2. Apply the same transformation steps (e.g., promote headers, change data types).
    
3. Append them into one table called something like `Combined_Sales`.
    

---

### **📋 How to Use It**

1. In Power BI, choose **Get Data &gt; Folder**.
    
2. Browse to the folder containing your files.
    
3. Click **Combine & Transform Data**.
    
4. Power BI opens the **Combine Files** wizard.
    
5. Review the sample file and transformation steps.
    
6. Click **OK** to generate a query that processes all files.
    

Power BI automatically creates helper queries:

* **Transform Sample File**: Defines the transformation logic.
    
* **Combine Files**: Applies the logic to all files.
    
* **Parameter**: Stores the sample file name.
    

---

### **📝 Final Thoughts**

The **"Combine Files"** feature in Power BI Desktop is a must-know tool for anyone dealing with structured data across multiple files. It simplifies your workflow, enhances consistency, and prepares your data for powerful analysis—all with just a few clicks.

# Transform Tab

## **1 Transpose**

### 🔄 Transpose in Power Query (Transform Tab)

In Power BI's Power Query Editor, **Transpose** is a powerful tool under the **Transform** tab used to **flip your table's rows into columns and columns into rows**.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754497607808/7a1f5ad6-734c-42b0-8d5c-198fe02444f0.png align="center")

### 🧠 What It Does:

Transpose changes the orientation of your data:

* **Rows become columns**
    
* **Columns become rows**
    

### 🎯 Use Case Example:

Imagine you have data like this:

| Year | Q1 | Q2 | Q3 | Q4 |
| --- | --- | --- | --- | --- |
| 2024 | 100 | 150 | 130 | 120 |

After **Transpose**, it becomes:

| Column1 | Column2 |
| --- | --- |
| Year | 2024 |
| Q1 | 100 |
| Q2 | 150 |
| Q3 | 130 |
| Q4 | 120 |

### ⚠️ Important Notes:

* Transpose works **on the entire table**, not on selected columns.
    
* It’s useful when you receive data in the wrong orientation from Excel or other sources.
    

## **2 Reverse Rows**

### 🔁 Reverse Rows in Power Query (Transform Tab)

Sometimes the order of rows matters—especially in time-series data or ordered categories. Power BI offers a simple but powerful tool called **Reverse Rows** under the **Transform** tab.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754497952065/fd10302c-f8da-4fd3-9e48-b5345456caeb.png align="center")

### 🧠 What It Does:

**Reverse Rows** flips the order of your entire table **from bottom to top**:

* The **last row becomes the first**
    
* The **first row becomes the last**
    

### 🎯 Use Case Example:

You start with:

| Index | Value |
| --- | --- |
| 1 | A |
| 2 | B |
| 3 | C |

After applying **Reverse Rows**, it becomes:

| Index | Value |
| --- | --- |
| 3 | C |
| 2 | B |
| 1 | A |

### 💡 When to Use:

* To reverse chronological order (e.g., showing latest dates first).
    
* After **sorting** if you want to flip the result.
    
* In **data preparation for visualizations or custom logic**.
    

### ⚠️ Note:

* It affects the **entire table**, not a single column.
    
* There's no setting panel—it's a one-click transformation.
    

## 3 Count Rows

### 🔢 Count Rows in Power Query (Transform Tab)

When working with large datasets, it's often useful to quickly determine the number of rows in a table. Power BI’s Power Query provides a simple one-click solution for this: **Count Rows**.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754498164985/11528f62-5b66-4409-bd0b-2a41f9065051.png align="center")

### 🧠 What It Does:

**Count Rows** calculates the **total number of rows** in the current query and returns that count as a **new single-row table** with one column.

### 🎯 Example:

Suppose your table has 250 rows of customer records.

After clicking **Count Rows**, Power Query will output:

| Count |
| --- |
| 250 |

This result **replaces your original table**, turning it into a single summary row.

## **4 Detect Data Type**

### 🧠 Detect Data Type in Power Query (Transform Tab)

Power Query often tries to guess the data type of each column when you load a dataset—but sometimes, you’ll need to do it manually or recheck. That’s where the **Detect Data Type** feature comes in handy.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754498633314/d3f86f38-8af3-4ec5-bd52-0b6a2b483545.png align="center")

### 🎯 Example:

If a column looks like this:

| Value |
| --- |
| 01/01/2024 |
| 05/03/2024 |

Power Query might detect and convert it to **Date** type.

Or if you have:

| Value |
| --- |
| 100 |
| 200 |

It could detect this as a **Whole Number** or **Decimal Number**.

### 💡 Use Cases:

* After importing data from Excel, CSV, or web, especially when data types are not automatically assigned.
    
* To quickly correct **“Any”** typed columns to their actual data type.
    
* When copying data from mixed sources with inconsistent formatting.
    

### ⚠️ Notes:

* It applies **automatically to all columns** unless you select a specific column first.
    
* If detection fails or is incorrect, you can manually change the data type using the **Data Type dropdown** next to column headers.
    

## **5 Rename**

### Rename in Power Query (Transform Tab)

When preparing data, clear and meaningful column names are crucial. The **Rename** feature in Power Query lets you quickly update column headers to improve readability and context.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754498889572/8cce0a79-0db3-4782-9d15-075161374b92.png align="center")

### 🧠 What It Does:

**Rename** allows you to **change the name of the currently selected column**.

You can also do this by:

* Double-clicking the column name directly, or
    
* Right-clicking the column header and selecting “Rename”.
    

### 🎯 Use Case Example:

You import a dataset and see:

| Column1 | Column2 |
| --- | --- |
| John | 200 |
| Sarah | 180 |

After renaming:

| Name | Score |
| --- | --- |
| John | 200 |
| Sarah | 180 |

### ⚠️ Tip:

If you rename a column that is used in later steps, Power Query **automatically updates** all dependent steps using that new name—**no need to worry about breaking your query**.

## 6 Replace Values

### 🔁 Replace Values & Replace Errors in Power Query (Transform Tab)

Cleaning up messy data is a common part of any data transformation workflow. Power Query gives you handy tools to quickly **replace specific values or fix error cells** in your dataset.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754529893730/73eaf625-fd43-48f5-8c22-32c9b3fe178a.png align="center")

### 🔄 **Replace Values**

#### 🧠 What It Does:

Lets you **find and replace specific values** within the selected column.

#### 🧪 Example:

| Value |
| --- |
| Yes |
| No |
| Yes |

➡ After replacing “Yes” with “1” and “No” with “0”:

| Value |
| --- |
| 1 |
| 0 |
| 1 |

#### ✅ Use Cases:

* Standardizing values (e.g., “Y” → “Yes”, “N” → “No”).
    
* Correcting typos or inconsistent entries.
    
* Preparing binary or numeric values for analysis.
    

### ⚠️ **Replace Errors**

#### 🧠 What It Does:

Allows you to **replace all error values** in a column with a custom value (e.g., 0, “Unknown”, “N/A”).

#### 🧪 Example:

| Sales |
| --- |
| 200 |
| Error |
| 350 |

➡ Replace Errors with “0”:

| Sales |
| --- |
| 200 |
| 0 |
| 350 |

#### ✅ Use Cases:

* Handling missing data or calculation errors.
    
* Preventing errors from breaking downstream steps.
    
* Displaying user-friendly alternatives to error messages.
    

### 💡 Pro Tip:

Always verify why errors exist before replacing them. You can use **“Keep Errors”** or **“Remove Errors”** (under the **Home** tab) to investigate.

## 7 Fill

### ⬇️⬆️ Fill Down & Fill Up in Power Query (Transform Tab)

When working with tabular data, especially exported or semi-structured files, you may encounter **missing values** in cells that should carry down or up from previous/next rows. Power Query solves this with the **Fill** tool.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754530496406/ebdbf0fc-89e7-4c3d-b949-7e89ac78638f.png align="center")

### 🔽 Fill Down

#### 🧠 What It Does:

Copies the **value from the row above** into blank (null) cells **below** it in the same column—until it hits the next non-null value.

#### 🧪 Example:

Before:

| Category | Value |
| --- | --- |
| Fruits | 10 |
| (null) | 20 |
| (null) | 30 |
| Veggies | 15 |

After Fill Down:

| Category | Value |
| --- | --- |
| Fruits | 10 |
| Fruits | 20 |
| Fruits | 30 |
| Veggies | 15 |

---

### 🔼 Fill Up

#### 🧠 What It Does:

Copies the **value from the row below** into blank (null) cells **above** it in the same column—until it hits the next non-null value.

#### 🧪 Example:

Before:

| Category | Value |
| --- | --- |
| (null) | 10 |
| (null) | 20 |
| Fruits | 30 |

After Fill Up:

| Category | Value |
| --- | --- |
| Fruits | 10 |
| Fruits | 20 |
| Fruits | 30 |

---

### 💡 Use Cases:

* Clean datasets from merged Excel cells (headers only shown once).
    
* Prepare grouped data for filtering, pivoting, or analysis.
    
* Ensure consistent category or label propagation in reports.
    

---

### ⚠️ Tips:

* Fill only affects **null/blank cells**, not zero or text like "N/A".
    
* Works **per column**, so apply separately if needed.
    

## 8 Pivot Column

### 📊 Pivot Column in Power Query (Transform Tab)

Need to turn row values into column headers? That’s exactly what the **Pivot Column** feature does in Power BI’s Power Query Editor—perfect for reshaping and summarizing data.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754530922411/bad40f22-665c-4cf5-b631-89d5f2eaed0e.png align="center")

### 🧠 What It Does:

**Pivot Column** transforms **distinct values in a selected column into new column headers**, and fills the table with related values from another column.

### 🎯 Example:

Original table:

| Month | Category | Sales |
| --- | --- | --- |
| Jan | Fruits | 100 |
| Jan | Veggies | 80 |
| Feb | Fruits | 120 |
| Feb | Veggies | 90 |

You pivot the **Category** column using **Sales** as values:

| Month | Fruits | Veggies |
| --- | --- | --- |
| Jan | 100 | 80 |
| Feb | 120 | 90 |

---

### ✅ Use Cases:

* Convert tall/narrow data into wide format.
    
* Create summary tables (e.g., months as rows, product types as columns).
    
* Better structure your data for reporting or charting.
    

### ⚠️ Notes:

* You must **specify the values column** to fill the pivoted headers.
    
* If multiple values exist for the same combination, Power Query will prompt you to **aggregate** (e.g., sum, average, count).
    
* Best used on **categorical columns** with **repeating labels**.
    

## 9 Unpivot Columns

### 🔄 Unpivot Columns in Power Query (Transform Tab)

While pivoting turns rows into columns, **Unpivoting** does the opposite—it helps **normalize wide tables** by turning column headers into row values. Power Query provides three flexible unpivoting options.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754531577309/7548f25f-15fb-4e1f-abf0-935fa91a614e.png align="center")

### 🔽 Options Explained:

#### 1️⃣ **Unpivot Columns**

* Unpivots only the **selected columns**.
    
* Ideal when you manually choose which columns should become row values.
    

**Example:**  
Original:

| Year | Jan | Feb |
| --- | --- | --- |
| 2024 | 100 | 120 |

Unpivot Jan & Feb ➜

| Year | Attribute | Value |
| --- | --- | --- |
| 2024 | Jan | 100 |
| 2024 | Feb | 120 |

---

#### 2️⃣ **Unpivot Other Columns**

* Keeps selected columns as **row identifiers**.
    
* For example, “Region” and “Product“ will be selected in this example.
    
* All **non-selected columns** are unpivoted.
    

**Useful when** you only want to preserve a few columns and unpivot the rest.

| Region | Product | Jan | Feb | Mar |
| --- | --- | --- | --- | --- |
| North | Apples | 100 | 120 | 110 |
| North | Bananas | 90 | 100 | 105 |
| South | Apples | 95 | 115 | 120 |

---

| Region | Product | Attribute | Value |
| --- | --- | --- | --- |
| North | Apples | Jan | 100 |
| North | Apples | Feb | 120 |
| North | Apples | Mar | 110 |
| North | Bananas | Jan | 90 |
| North | Bananas | Feb | 100 |
| North | Bananas | Mar | 105 |
| South | Apples | Jan | 95 |
| South | Apples | Feb | 115 |
| South | Apples | Mar | 120 |

#### 3️⃣ **Unpivot Only Selected Columns**

* Same as **Unpivot Columns** — added for clarity and usability.
    
* Appears more explicitly when using contextual right-click options.
    

---

### ✅ Use Cases:

* Normalize cross-tab reports (e.g., monthly sales as columns).
    
* Prepare data for dynamic analysis and visualizations.
    
* Load Excel-like wide tables into a more database-friendly long format.
    

### ⚠️ Tips:

* After unpivoting, Power Query creates two new columns:
    
    * **Attribute** (previous column names)
        
    * **Value** (cell values)
        
* Rename these columns to something meaningful (e.g., "Month" and "Sales").
    

## 10 Move

### 🔀 Move Columns in Power Query (Transform Tab)

When cleaning or organizing data, the **order of columns** can matter for readability or functionality. Power Query makes it easy to move columns around with the **Move** tool under the **Transform** tab.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754534780035/a7597613-d737-48b3-9d9e-00a575963065.png align="center")

### 🧠 What Each Option Does:

| Option | Action |
| --- | --- |
| **Left** | Moves the selected column one position to the left. |
| **Right** | Moves the selected column one position to the right. |
| **To Beginning** | Sends the selected column to the first position in the table. |
| **To End** | Sends the selected column to the last position. |

### ✅ Use Cases:

* Group related columns together (e.g., IDs, dates, values).
    
* Improve visual clarity when viewing data in Power BI.
    
* Prepare data for pivoting or exporting in a specific format.
    

### 💡 Tips:

* Works with **one column at a time** (multi-select isn't supported).
    
* You can also **drag-and-drop** columns manually, but the **Move tool** ensures consistency and keeps steps recorded in the Applied Steps pane.
    

## **11 Convert to List**

### 📜 Power Query – Convert to List

The **Convert to List** option in Power BI’s Power Query editor allows you to transform a single column into a **flat list** — removing the table structure and returning just the values.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754536524366/fda128fa-bf49-4839-a747-358088b16437.png align="center")

### 🔍 What Does It Do?

When you select a single column and click **Convert to List**, Power Query:

* Removes the table structure
    
* Returns the selected column’s values as a **list object**
    

Example output:

```plaintext
{"Apple", "Mango", "Orange"}
```

### ✅ When to Use:

* You need to **extract a list of values** from a column
    
* You're building a **custom function** that takes a list as input
    
* You want to use this list in **comparisons, filters, or joins**
    

### 🧪 Example:

#### Original Table:

| Product |
| --- |
| Apple |
| Mango |
| Orange |

#### After Convert to List:

```plaintext
{"Apple", "Mango", "Orange"}
```

You can then use this list in:

* Lookup logic
    
* Filtering another table
    
* Creating parameters
    

### ⚠️ Notes:

* Only works with **one column** at a time
    
* The result is **no longer a table** — it becomes a list type
    
* You’ll need to use **advanced editor or steps** if you want to bring it back into a table
    

## Run R Script

### 🧬 Power Query – Run R Script

The **“Run R Script”** option in Power BI’s Power Query Editor allows you to run **R code** directly on your dataset for advanced data transformation, statistical analysis, or visualization preparation.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754618602209/827d587a-bd60-4ef9-9c54-0924052f522f.png align="center")

### 🛠️ What Does It Do?

This tool lets you:

* Leverage **R’s rich statistical capabilities**
    
* Apply **custom R transformations**
    
* Integrate R-powered models or functions into your Power BI data
    

When you click **Run R Script**:

1. A script editor opens
    
2. You write or paste R code
    
3. Power Query runs that R code on your current dataset
    

---

### ✅ Requirements:

* **R must be installed** on your machine
    
* Configure R path via **File &gt; Options &gt; R Scripting**
    
* R script execution must be enabled
    

### 🧪 Example Use Case:

Imagine you want to **remove outliers** using R:

```plaintext
dataset <- dataset[abs(scale(dataset$Value)) < 3, ]
```

This line filters out rows where the "Value" column is more than 3 standard deviations from the mean.

> The input data is always accessible in R through a variable named `dataset`.

### 🔒 Security Note:

Power BI disables script execution for files from untrusted sources unless explicitly enabled.

---

### 📊 Why Use R in Power BI?

* Advanced statistics (e.g., regression, clustering)
    
* Complex data reshaping
    
* Leverage existing R scripts/models
    
* Visualization prep using R packages
    

# Add Column

## 1 Column From Examples

**"Column From Examples"** lets you *generate a new* column by providing sample values based on existing data. Power BI analyzes the logic behind your examples and automatically creates the M code to replicate that transformation.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754298937176/9ae62c31-bd01-49b3-a897-e83990e9fcaf.png align="center")

* Go to the Add Column tab.
    
* Click Column From Examples.
    
* Choose:
    

From All Columns – Suggests transformations using all available columns.

From Selection – Suggests based on only the columns you select beforehand.

* In the new interface, type the expected output (your example values) row by row.
    
* Power BI will detect the pattern and generate the formula automatically.
    
    ### From Selection
    

**✅ Example Use Case:**

You have a Full Name column like:  
"**JOHN SMITH**"

You want to create a column with just the first name in proper case:  
Type "John" in the first row → Power BI auto-detects you want the proper-case first name and generates the logic for it.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754299006413/725a766a-9ad8-4b94-8496-53e618e8d1ac.png align="center")

**Result**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754299081850/f40c7201-b226-417e-98ed-dd4267a99b3d.png align="center")

### From all columns

Real-World Use Case: Create a Personalized Email Greeting

You want to generate a personalized greeting line for each customer that looks like this:

**"Hello Mary, your can collect your Power Bank from New York."**

This output depends on multiple columns:

* First name → from Full Name
    
* Product → from Product
    
* City → from City
    

**🛠 Steps to Perform This in Power BI:**

1. **Go to:**  
    Add Column &gt; Column From Examples &gt; From All Columns
    
2. **In the new column** (right side), type:
    

Hello **JOHN SMITH**, you can collect your **Power Bank** from **New York**.

3. As soon as you start typing, Power BI tries to detect which columns you're using and auto-fill the rest.
    
4. Check if Power BI got the pattern right for rows 2 and 3:
    

Hello **JOHN SMITH**, you can collect your **Power Bank** from **New York**.

Hello **MARY JOHNSON**, you can collect your **Wireless Mouse** from **Chicago**.

4. **Click OK** to confirm.
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754299107598/781d13a6-a554-4c78-8ec6-144f9283ca21.png align="center")

**Result**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754299135997/9a0cf39f-d4dc-4965-acce-7f2b597313df.png align="center")

## 2 Custom Column

The **Custom Column** tool in Power BI (under the **Add Column** tab) allows you to **write a formula using M language** to define a new column based on logic, math, string operations, or conditions using existing columns.

Unlike *Column From Examples* (which infers logic based on what you type), **Custom Column gives you full control** by letting you write the logic manually.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754304484231/71756c43-bdac-4ac6-9c73-49566a2030c6.png align="center")

### 📌 How to Use It

1. Go to **Add Column &gt; Custom Column**.
    
2. A dialog box opens where you:
    
    * Give your new column a name.
        
    * Write a formula using Power Query M Language.
        
3. Click **OK** — a new column is added based on your logic.
    

### 💡 Why Use Custom Column?

* Precise control over logic and output.
    
* Write complex conditions and calculations.
    
* Handle text, numbers, dates, or even conditional logic like `if...then...else`.
    

### 💡 Explanation:

* `[Full Name]`: Refers to the original uppercase name.
    
* `Text.Proper(...)`: Capitalizes each word (e.g., JOHN SMITH → John Smith).
    
* `" - "`: Adds a separator.
    
* `[City]`: Gets the city name.
    
* `Text.Upper(...)`: Converts city to all caps (e.g., New York → NEW YORK).
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754304304160/1dd6d808-6f26-4182-804b-532eede98286.png align="center")

**Result**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754304721238/3a41a684-b0b1-4ddd-91e0-47ec55e0a72d.png align="center")

## **3 Invoke Custom Function**

**Invoke Custom Function** allows you to call (or "invoke") a **custom Power Query function** on a row-by-row basis, using values from your existing table as inputs.

Think of it like applying a mini-program (function) to each row of your table — just like using a formula in Excel, but written in **M language** and reusable across queries.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754313488126/8f976ff5-c75b-4c4c-bd76-07eb95147f23.png align="center")

### 📌 When to Use It:

* You’ve created a **custom function** in Power Query (like a reusable step).
    
* You want to apply that logic across a dataset using different input values from your columns.
    

---

### ✅ Real Example: Add Sales Tax Based on City

#### 🎯 Scenario:

You’ve written a **custom function** that calculates tax based on city name (e.g., different cities have different tax rates).  
You want to apply this function to each customer row based on the `City` column.

### Create a New Blank Query

In the **Queries pane (left side)**:

1. Right-click anywhere in the blank space or on any query name.
    
2. Select **New Query &gt; Blank Query**.
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754312136963/0b72c6d1-729e-4135-af1d-41637ce4624f.png align="center")

### Open the Advanced Editor

1. With the new blank query selected, go to **Home &gt; Advanced Editor**.
    
2. Replace the placeholder code with your custom function.
    

### ✏️ Sample Function: Get Tax Rate by City

```plaintext
(city as text) as number =>
    if city = "New York" then 0.08
    else if city = "Los Angeles" then 0.09
    else 0.05
```

This function takes a `city` as input and returns the applicable tax rate.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754312423288/7d7775bd-818e-4b06-bcb0-37a728bf84d9.png align="center")

### Rename It as a Function

* In the **Properties pane** (right side or via right-click), rename the query to something meaningful like:  
    `GetCityTaxRate`
    

### 🧪 How to Test It (Optional Step):

* You can type a city like `"New York"` into the input box and click **Invoke** to manually test it.
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754312748266/d59ee5c6-bfc7-4183-b2c8-e4348009d7e8.png align="center")

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754312874008/d01a3eef-8c61-4622-9729-74f0a64e868a.png align="center")

### Invoke the Function on a Table

1. Go back to your **main table** (e.g., `Customers`).
    
2. Go to **Add Column &gt; Invoke Custom Function**.
    
3. In the dialog:
    
    * Name your new column.
        
    * Choose the function you just created (`GetCityTaxRate`).
        
    * Map the `City` column as the input.
        
4. Click **OK**.
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754313125420/5cbbfe34-242b-4d99-a425-e279257eb002.png align="center")

**Result**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754313242064/6cddfe88-4be8-402a-92d6-1e4864db91fa.png align="center")

## 4 **Conditional Column**

### 📌 What it does: *“If this, then that” logic*

Adds a new column where the value is based on **conditions** you define — similar to Excel’s **IF statements**.

### 🛠 Example Use Case:

You want to label customers based on city:

> If the `City` is `"New York"` then label them as `"East Coast"`, otherwise `"Other"`.

### 🔁 How to Use:

1. Click **Add Column &gt; Conditional Column**.
    
2. Name the new column (e.g., `Region`).
    
3. Set your condition:
    
    * **If** `City` **equals** `"New York"` → then `"East Coast"`.
        
    * **Else** → `"Other"`
        
4. Click **OK**.
    

Power BI adds a new column with your defined labels.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754314267913/ae1cff32-84d1-45de-9ab6-dbb7c7c6256a.png align="center")

**Result**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754314504246/602ce0a4-8561-4bd6-a0d3-38a78e41ac4c.png align="center")

## 5 **Index Column**

### 📌 What it does:

**Index Column** adds a **sequential number column** to your table — basically assigning a row number to each record.

Think of it as **“Row ID”** — it starts from 0 or 1 and increases by 1 (or any custom step you define).

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754315108331/5b24fd55-c2f3-4985-9b64-004286ff9561.png align="center")

### 🛠 Where to find it:

**Add Column &gt; Index Column**  
You’ll see a dropdown with:

* **From 0** → Starts numbering at 0
    
* **From 1** → Starts numbering at 1
    
* **Custom** → You choose both start value and step size
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754315199919/a5db601d-2343-448c-9204-a22aeef8c526.png align="center")

**Result**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754315270398/137e7648-b491-49e1-bb5f-7f5c8eac8d22.png align="center")

## 6 **Duplicate Column**

### 📌 What it does:

**Duplicate Column** makes an exact copy of the selected column and adds it to your table. The new column is named `OriginalName - Copy` by default.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754315695396/80d01000-fca8-4223-ac44-751df0ee5b5f.png align="center")

### 🛠 Where to find it:

**Add Column &gt; Duplicate Column**

✅ Why It’s Useful:

You can **safely apply transformations** (e.g., formatting, splitting, cleaning) to the copy without changing the original data.

| Use Case | Benefit |
| --- | --- |
| Keep original data untouched | For auditing or backup |
| Test transformations on a copy | Try proper case, splits, trim, etc. |
| Run comparisons | Before/after logic, detect changes |

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754315790962/ae9c75be-011c-4069-ab32-ce477c310a81.png align="center")

## **7 Format (ABC)**

### 📌 What it does:

The **Format** tool applies **text-based transformations** to a column (like changing case or cleaning up characters). It's especially useful when working with messy or unstructured data.

Each option creates a **new column** (because you’re in the **Add Column** tab) with the applied formatting.

### 🛠 Options Explained:

| Option | What It Does | Example |
| --- | --- | --- |
| **lowercase** | Converts all text to lowercase | `"JOHN DOE"` → `john doe` |
| **UPPERCASE** | Converts all text to uppercase | `"John Doe"` → `JOHN DOE` |
| **Capitalize Each Word** | Proper case — capitalizes the first letter of each word | `"john DOE"` → `John Doe` |
| **Trim** | Removes **leading and trailing spaces** | `" John "` → `John` |
| **Clean** | Removes **non-printable/invisible characters** like line breaks or hidden symbols | `"Jo\u0003hn"` → `John` |
| **Add Prefix** | Adds text at the **start** of each value | `"Name :"` + `JOHN SMITH-` → `Name : JHON SMITH` |
| **Add Suffix** | Adds text at the **end** of each value | `"@hotmail.com"` + JOHN SMITH → JOHN SMITH@hotmail.com |

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754318017352/cddecc92-a31f-4aae-9494-e8d83de95140.png align="center")

**Result**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754318111585/94c9777a-8895-4251-ad2e-24071e715d9a.png align="center")

## **8 Merge Columns**

### 📌 What it does:

**Merge Columns** lets you **combine the values of two or more columns** into a single column — with or without a separator (like space, dash, or custom text).

It's useful for creating full names, addresses, product codes, or any custom labels from multiple fields.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754318909317/b9386acb-8b62-4a97-8b91-8a96ce7ae4a6.png align="center")

### 💡 Tip:

**Column order matters** — Power BI merges values **in the order you selected them**.

So:

* Select `Prefix`, then `First Name`, then `Last Name` → gets you: `Mr. John Smith`
    
* Select in reverse → gets: `Smith John Mr.`
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754319025103/75db8a56-34a8-48c0-9ffb-8a980559fd1a.png align="center")

Result

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754319114301/bc7d0f28-8aee-4556-8656-48fca3532610.png align="center")

## **9 Extract**

### 📌 What it does:

The **Extract** tool allows you to **pull out parts of a text string** — such as:

* First characters
    
* Last characters
    
* Substrings before/after a delimiter
    

This is useful when you're working with compound strings like `"CUST-123"` or `"`[`john.doe@example.com`](mailto:john.doe@example.com)`"` and want to isolate a portion of it.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754319427578/edaed8e6-737f-4302-9231-0861d2f1ca4e.png align="center")

---

### 🧰 Options in the Extract Menu:

| Option | What it Does | Example |
| --- | --- | --- |
| **First Characters** | Extracts the first N characters | `ABC123` → `ABC` |
| **Last Characters** | Extracts the last N characters | `ABC123` → `123` |
| **Range** | Extracts characters from a specific **start position** and **count** | From position 2, extract 3 → `ABC123` → `BC1` |
| **Text Before Delimiter** | Gets all text before a specified character or symbol | [`john.doe@example.com`](mailto:john.doe@example.com) → `john.doe` (before `@`) |
| **Text After Delimiter** | Gets all text after a specified character or symbol | `CUST-123` → `123` (after `-`) |
| **Text Between Delimiters** | Extracts the text between two delimiters | `Hello [World]!` → `World` (between `[` and `]`) |

**Result**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754319950401/82f971e2-fe5c-426b-a812-88718e916262.png align="center")

## **10 Parse (XML / JSON)**

### 📌 What it does:

The **Parse** tool allows you to **convert a column containing XML or JSON text** into a **structured record or table format** that you can work with in Power BI.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754321338332/39c15e30-07e8-48f5-9286-4c15e945f83d.png align="center")

### 🔍 When to Use:

Use **Parse** when you have:

* A column with XML or JSON **text strings**
    
* Embedded structured data inside a single column
    
* Output from APIs, logs, nested exports, or IoT sensors
    

---

### 📂 Parse Options:

| Option | Purpose | Example |
| --- | --- | --- |
| **XML** | Converts XML-formatted text to a hierarchical record | `<customer><name>John</name></customer>` |
| **JSON** | Converts JSON-formatted text to records/tables | `{ "name": "John", "city": "New York" }` |

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754321432623/643811fd-f7ad-4965-b76b-e51ba59950a2.png align="center")

**Result JSON**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754321508145/f3d1f9fe-a154-4a2c-9f01-b503e0bcab47.png align="center")

**Result XML**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754321689483/83de0818-4d3f-4a42-b7f5-8037f89681fd.png align="center")

## **11 Statistics Tool**

### 📌 What it does:

The **Statistics** tool allows you to **generate basic statistical summaries** from numeric columns — like mean, min, max, standard deviation, and more — **on a row-by-row basis or across the entire column** (depending on context).

In Power Query, it is mainly used to **create a new column** that contains a calculated value based on existing numeric data.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754322240154/76351dea-fb5c-4c2c-b25f-798690642267.png align="center")

---

### 📂 Common Options in the Dropdown:

| Option | What it Calculates |
| --- | --- |
| **Minimum** | The smallest value in the column |
| **Maximum** | The largest value in the column |
| **Average** | The mean of the values |
| **Median** | The middle value |
| **Standard Deviation** | Spread of the values from the mean |
| **Count Values** | Number of non-null values |
| **Sum** | Total of all values |

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754322470831/280c982b-ff4f-4f1f-840f-1ceb1a00478f.png align="center")

**Result**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754322572100/c760113a-6572-45fe-b89c-5eccd69b035e.png align="center")

## **12 Standard (Math Operations)**

### 📌 What It Does:

The **Standard** dropdown lets you apply row-level **mathematical operations** on numeric columns like:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754352336590/db8c9c44-2aec-4c5f-989d-3ed1e5fbd7a3.png align="center")

| Operation | What It Does |
| --- | --- |
| **Add** | Sums selected columns row-by-row |
| **Multiply** | Multiplies selected column values |
| **Subtract** | Subtracts one column from another |
| **Divide** | Divides one column by another |
| **Divide (Integer)** | Integer division (no decimal) |
| **Modulo** | Remainder after division |
| **Percentage** | Calculates percentage of one column to another |
| **Percent Of** | Same as percentage, phrased differently |

## **13 Scientific Operations**

### 📌 What It Does:

The **Scientific** dropdown lets you apply **scientific and mathematical functions** (like powers, roots, logs, etc.) on numeric columns — row by row — and adds the result as a new column.

---

### 🧰 Available Options & What They Do:

| Operation | Description | Example |
| --- | --- | --- |
| **Absolute Value** | Removes minus sign (converts to positive) | `-500 → 500` |
| **Power** &gt; *Power of N* | Raises each number to a given power | `2^3 = 8` |
| **Square Root** | Calculates square root of each value | `√9 = 3` |
| **Exponent** | Calculates **e^x** for each value | `e^2 ≈ 7.39` |
| **Logarithm** &gt; *Base 10 / Base e* | Calculates the log of each value | `log10(1000) = 3` |
| **Factorial** | Computes factorial `n!` for each value | `5! = 120` |

### ⚠️ Caution:

* Only works on **numeric columns**.
    
* **Factorial** is best used for **small whole numbers** (it grows very fast!).
    
* **Logarithms** and **roots** of negative numbers or zero will throw errors.
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754353303595/3315b1e5-2580-4fba-9974-50568f4a502e.png align="center")

## 14 T**rigonometry Functions**

### 📌 What it does:

The **Trigonometry menu** allows you to apply **trigonometric functions** (like sine, cosine, tangent, etc.) to **numeric columns**. These are applied row-by-row, and a new column is added with the results.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754356911181/c728bca8-dcdb-41be-9f6c-75cd4f62404d.png align="center")

---

### 🧮 Available Functions:

| Function | Description |
| --- | --- |
| **Sine** | Returns the sine of the input (in radians) |
| **Cosine** | Returns the cosine of the input (in radians) |
| **Tangent** | Returns the tangent of the input (in radians) |
| **Arcsine** | Returns the angle (in radians) whose sine is the input |
| **Arccosine** | Returns the angle whose cosine is the input |
| **Arctangent** | Returns the angle whose tangent is the input |

---

### 📘 Practical Usage:

| When it's useful | Example |
| --- | --- |
| Geometry modeling | Map GPS, shapes, or trajectories |
| Engineering data | Use sine/cosine for waveform signals |
| Scientific research | Perform angle-based calculations |

## **15 Rounding Functions**

### 📌 What it does:

The **Rounding** tool lets you control how numeric values are rounded by creating a new column with the adjusted values.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754357090390/4361103b-6c30-4b4e-a11c-64b768eaf0af.png align="center")

### 🧰 Options Explained:

| Option | What it Does | Example (Input = 12.76) |
| --- | --- | --- |
| **Round Up** | Rounds up to the nearest integer (ceiling) | `13` |
| **Round Down** | Rounds down to the nearest integer (floor) | `12` |
| **Round...** | Opens a dialog box where you can specify the **number of decimal places** to round to | `Round to 1 decimal = 12.8` |

---

### 🧪 Example Use Case:

You have a column: `Bonus %` = `12.76489`

You want to:

* Round to **2 decimal places** → Use **Round…**
    
* Round **up to nearest whole number** → Use **Round Up**
    
* Round **down to nearest whole number** → Use **Round Down**
    

## **16 Information Functions**

### 📌 What it does:

The **Information** tool helps you create new columns that **evaluate properties of numeric values** — like whether they’re even, odd, or what their sign is (positive/negative/zero).

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754357491724/c2b13645-abf0-4f85-b9c4-1ba65f4b712d.png align="center")

---

### 🔍 Options in the Menu:

| Option | Description | Example Input | Output |
| --- | --- | --- | --- |
| **Is Even** | Returns `true` if the number is even | `4` | `true` |
| **Is Odd** | Returns `true` if the number is odd | `3` | `true` |
| **Sign** | Returns: `1` (positive), `-1` (negative), `0` (zero) | `-5` | `-1` |

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754357810899/0f727b7e-0d21-4b36-9bb4-cbcc3d43296c.png align="center")

## 17 Date Transformations

Power BI's **Power Query Editor** offers powerful tools to analyze and manipulate dates. One of the most essential menus under the **Add Column** tab is the **Date** dropdown. This guide walks you through every option available, using real-world scenarios to help you transform your date columns into insights.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754358869347/99207c49-5ec5-4309-b315-a0685e975a17.png align="center")

## 📒 Real-World Use Cases

### Example Table

| Order\_ID | Order\_Date |
| --- | --- |
| ORD100 | 8/5/2024 |
| ORD101 | 6/15/2024 |
| ORD102 | 1/23/2024 |
| ORD103 | 11/10/2023 |
| ORD104 | 12/31/2023 |

## 📅 Full Reference: Date Menu Options with Examples

| Group | Option | Description | Example Date (2024-08-05) | Result |
| --- | --- | --- | --- | --- |
| **General** | `Age` | Calculates duration from the date to today. | 2024-08-05 | 365.07:00:00 |
|  | `Date Only` | Removes time, keeping only date. | 2024-08-05 12:00:00 | 2024-08-05 |
| **Parse** | *(Grayed out)* | Used to convert text to date format. | (text) | N/A |
| **Year** | `Year` | Extracts the year. | 2024-08-05 | 2024 |
|  | `Start of Year` | First day of the year. | 2024-08-05 | 2024-01-01 |
|  | `End of Year` | Last day of the year. | 2024-08-05 | 2024-12-31 |
| **Month** | `Month` | Returns the numeric month. | 2024-08-05 | 8 |
|  | `Name of Month` | Returns full month name. | 2024-08-05 | August |
|  | `Start of Month` | First day of the month. | 2024-08-05 | 2024-08-01 |
|  | `End of Month` | Last day of the month. | 2024-08-05 | 2024-08-31 |
| **Quarter** | `Quarter` | Returns quarter name. | 2024-08-05 | Q3 |
|  | `Start of Quarter` | First day of the quarter. | 2024-08-05 | 2024-07-01 |
| **Week** | `Week of Year` | ISO week number of the year. | 2024-08-05 | 32 |
|  | `Week of Month` | Which week of the month it falls in. | 2024-08-05 | 1 |
|  | `Start of Week` | First day of the current week. | 2024-08-05 | 2024-08-05 (Monday) |
| **Day** | `Day` | Day of the month. | 2024-08-05 | 5 |
|  | `Name of Day` | Full weekday name. | 2024-08-05 | Monday |
|  | `Day of Week` | Number representing day of week (0 = Sunday). | 2024-08-05 | 1 |
|  | `Day of Year` | Day number of the year. | 2024-08-05 | 218 |
| **Calculation** | `Subtract Days` | Subtracts fixed number of days. | 2024-08-05 - 3 days | 2024-08-02 |
| **Combine** | `Combine Date and Time` | Merges date and time columns into DateTime. | 2024-08-05 + 10:00 AM | 2024-08-05 10:00:00 |
| **Boundary Dates** | `Earliest` | Earliest date from selected column. | ORD104 to ORD100 | 2023-11-10 |
|  | `Latest` | Latest date from selected column. | ORD104 to ORD100 | 2024-08-05 |

---

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754358790195/9e0264a0-47df-45be-b728-b83a4413e496.png align="center")

## 🔧 Tips for Best Use

* Always convert your date/time fields to the correct type (`Date` or `Date/Time`).
    
* Use **"Add Column"** if you want to keep the original column.
    
* Use **"Transform"** if you want to overwrite the column with a new result.
    
* Use **Age** and **Subtract Days** together to calculate delivery duration, account age, or follow-up time.
    

---

## 🌟 Final Thoughts

The Date menu in Power BI unlocks deep time-based insights with just a few clicks. Mastering these transformations empowers you to build **powerful date intelligence**, seasonal analysis, and time-driven dashboards.

## 18 Time Functions

Working with time data in Power BI can unlock deeper insights into customer behavior, event trends, and operational performance. In this post, we'll walk through how to use **Power Query Editor's Time tools** to extract, calculate, and combine time values using real use cases.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754362741076/5dd2675d-6357-4252-bd6d-b89b4e558f45.png align="center")

## 🕐 Extracting Time Parts

You can split a DateTime column into meaningful parts:

### ✅ Example:

From a column like `Event_Timestamp`, we can extract:

* **Hour**: e.g., 9:30 AM → `9`
    
* **Minute**: e.g., 9:30 AM → `30`
    
* **Second**: e.g., 10:10:10 PM → `10`
    

## 🕓 Start and End of the Hour

You can also extract:

* **Start of Hour** – Trims the time to the beginning of the hour (e.g., 9:30 → 9:00)
    
* **End of Hour** – Rounds to the next full hour (e.g., 9:30 → 10:00)
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754362991182/b153d6bd-5797-48f0-b527-1bab7b098c7f.png align="center")

> ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754362869958/c8f624f0-914f-49c6-9cd2-5cabde577970.png align="center")

## ➗ Subtract Time Columns

Calculate the difference between two time columns using **Subtract** under the Time menu.

### ✅ Use Case:

If `Event_Time` is `9:30 AM` and `Event_Time-2` is `9:35 AM`, subtracting gives `00:05:00` (5 minutes).

## 🔁 Combine Date and Time

Got separate date and time columns? No problem.

Use **Combine Date and Time** to create a full `DateTime` field.

### ✅ Example:

* `Event_Date`: 8/5/2024
    
* `Event_Time`: 9:30 AM  
    ➡️ Combine to get: `8/5/2024 9:30:00 AM`
    

This is useful when merging logs or analyzing events by timestamp.

> 📸 *\[See Screenshot: Merged DateTime\]*

---

## 🔁 Compare Times: Earliest vs Latest

The **Earliest** and **Latest** tools help you pick the first or last time between two values.

### ✅ Example:

Between `Event_Time` and `Event_Time-2`, use:

* `Earliest` → smaller of the two
    
* `Latest` → greater of the two
    

This is handy when:

* Finding the true start time of an activity
    
* Prioritizing log entries
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754366246372/538ce2ae-3c46-4eb9-8fad-fee4b4c5fc21.png align="center")

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754366439562/320d08f5-eee1-4a73-86bf-e770a7ef6ebf.png align="center")

## ✅ Final Thoughts

Time transformations in Power BI’s Power Query Editor are intuitive and powerful. With just a few clicks, you can:

* Break apart timestamps
    
* Calculate durations
    
* Combine or compare moments
    
* Extract insights from raw event logs
    

These capabilities can turn basic datetime data into **actionable intelligence** for your dashboards and reports.

## 19 Duration Tools

Working with date and time in Power BI opens the door to powerful analysis — from customer behavior and system performance to detailed operational timing. In this post, we'll explore **Time** and **Duration** tools under the **Add Column** tab in Power Query Editor, with screenshots to guide you step-by-step.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754369588032/23acff3c-5599-4bcc-ba1c-c83519fef524.png align="center")

## ⏳ Duration Functions

Once you subtract two datetime columns, the result is a **duration value**. The **Duration** menu allows further breakdown and manipulation of this value.

### 🔧 Tools Available:

#### Breakdown:

* **Days**
    
* **Hours**
    
* **Minutes**
    
* **Seconds**
    
* **Total Years**, **Total Days**, **Total Hours**, etc.
    

#### Math Operations:

* **Subtract**
    
* **Multiply**
    
* **Divide**
    

#### Analysis:

* **Statistics** → Run operations like Min, Max, Median on duration fields
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754369680965/ac9cff50-e35a-454c-8dd9-47c5bc058387.png align="center")
    
    ## 20 Text Analytics
    
    Power BI isn’t just for numbers — it can also make sense of unstructured **text data** like customer feedback, support tickets, or survey responses. That’s where the **Text Analytics** feature in the Power Query Editor shines.
    
* ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754370531778/6ac27825-a6a1-4952-bf59-1403510841e4.png align="center")
    
* The **Text Analytics** tool leverages **Azure Cognitive Services** to apply natural language processing (NLP) to your data. With just a few clicks, you can:
    
    * ✅ **Detect Sentiment** (Positive, Negative, Neutral)
        
    * ✅ **Extract Key Phrases**
        
    * ✅ **Identify the Language**
        
    * ✅ **Detect Named Entities** (like names, places, and brands)
        
    
    No need to write code or use external tools — it’s all built right into the Power BI interface under the **Add Column &gt; Text Analytics** section.
    
    ---
    
    ## 🔐 Do You Need Premium?
    
    Yes. These AI-powered insights require either:
    
    * A **Power BI Premium** or **Premium Per User (PPU)** license  
        **OR**
        
    * A connected **Azure Cognitive Services** subscription (with an API key)
        
    
    Without one of these, the feature will remain inactive or prompt you to upgrade.
    
    ---
    
    ## 💡 Real-World Use Cases
    
    * 📊 **Customer Feedback Analysis**  
        See how your customers really feel using sentiment scores.
        
    * 📝 **Survey Text Summaries**  
        Extract recurring keywords and themes from open-ended responses.
        
    * 🧾 **Support Ticket Triage**  
        Auto-detect language or named entities for better routing.
        
    
    ---
    
    ## 21 Vision
    
    Power BI isn’t limited to structured data — it can also analyze **image files** using artificial intelligence. The **Vision** feature in the Power Query Editor brings **computer vision** to your BI workflow, powered by **Azure Cognitive Services**.
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754370783007/bcabba06-2dba-47ed-9984-8db7a158fe8f.png align="center")
    
    🔍 What is the Vision Tool?
    
    The **Vision** button in Power BI allows you to extract information from images using **Azure’s Computer Vision API**.
    
    With it, you can:
    
    * 🆔 **Extract Text (OCR)** from images like scanned forms or receipts
        
    * 🧠 **Analyze Image Content**, identifying objects or tags
        
    * 🗂️ **Describe Images** with automatically generated captions
        
    
    It turns unstructured image files into structured, reportable data.
    
    ---
    
    ## 🔐 Do You Need Premium?
    
    Yes — to use the Vision AI feature, you need:
    
    * A **Power BI Premium** or **Premium Per User (PPU)** license  
        **OR**
        
    * An **Azure Cognitive Services** subscription with a valid key
        
    
    Without this, the feature remains unavailable or prompts a connection setup.
    
    ---
    
    ## 💡 Real-World Use Cases
    
    * 📷 **Invoice OCR**  
        Extract invoice numbers, amounts, and dates from uploaded scans.
        
    * 🧾 **Receipt Processing**  
        Convert photographed receipts into structured datasets for expense tracking.
        
    * 🏷️ **Image Tagging**  
        Automatically tag and categorize marketing or product images.
        
    
    ---
    
    ## 🚀 Final Thoughts
    
    **Vision AI in Power BI** unlocks the power of image analysis within your data workflows. Whether you're digitizing paper records or analyzing image-heavy datasets, this feature can save time and improve data accessibility.
    
    If you're working with visuals and documents, this is one AI tool worth enabling.
    

## 22 Azure Machine Learning

Power BI’s true strength lies in combining business intelligence with artificial intelligence. The **Azure Machine Learning** button in the Power Query Editor lets you apply **trained ML models** directly to your data — no coding required.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754370885403/7590c8ff-39e6-4918-8c43-1de4dc45319a.png align="center")

The **Azure Machine Learning** option allows you to connect to models built and published in **Azure Machine Learning Studio**, and apply them to your datasets inside Power BI.

You can use it to:

* 🧠 Predict churn, customer behavior, or product returns
    
* 📈 Score leads using a trained classification model
    
* 📊 Apply clustering, regression, or time-series forecasts
    

It turns Power BI into a **real-time model consumer**, not just a report viewer.

---

## 🛠️ How Does It Work?

1. You build and train a model in **Azure Machine Learning Studio**.
    
2. Publish it as a **web service** (API endpoint).
    
3. In Power BI:
    
    * Click **Add Column &gt; Azure Machine Learning**
        
    * Authenticate with your Azure credentials
        
    * Choose the model and map the input columns
        
    * Power BI sends your data to the model and retrieves predictions
        

---

## 🔐 Do You Need Premium?

**No**, this feature does **not** require Power BI Premium.

However, you do need:

* An **Azure subscription**
    
* A **deployed machine learning model** in Azure Machine Learning Studio
    

---

## 💡 Real-World Use Cases

* 🏦 **Finance**: Predict loan default risk
    
* 🛒 **Retail**: Forecast sales volume or demand
    
* 📞 **Customer Support**: Predict ticket escalation
    
* 🌐 **Web Analytics**: Classify visitor intent
    

# VIEW

## **1 Query Settings**

### 🔧 Power BI Power Query Editor: Understanding the **Query Settings** Panel

When working in Power BI's **Power Query Editor**, one of the most important tools you’ll use is the **Query Settings** pane. This panel appears on the **right-hand side** of the screen and is essential for tracking and managing your data transformation steps.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754621946163/c0ffb837-d45f-4e59-9685-dbba6af30245.png align="center")

### 📌 What is the **Query Settings** Panel?

The **Query Settings** panel allows you to:

1. 🔍 **Rename and manage the current query**
    
2. 🧾 **View and edit all transformation steps** applied to the data
    
3. 📋 **Access properties** like table name, data source, etc.
    

### 🛠️ Two Key Sections:

#### 1️⃣ **PROPERTIES**

* **Name**: This is the name of the query/table.
    
* You can rename it here to something meaningful like `"July Issues"` instead of a generic name.
    
* Click **"All Properties"** to edit advanced settings like descriptions or annotations.
    

#### 2️⃣ **APPLIED STEPS**

This is where all the data transformation steps are listed in order. Each time you:

* Filter rows
    
* Rename columns
    
* Change data types
    
* Remove columns  
    …Power BI records that action here as a **step**.
    

Each step can be:

* **Edited** (by clicking the gear icon ⚙️ if available)
    
* **Reordered or deleted** (via right-click)
    
* **Used for debugging** if something breaks
    

### 💡 Why Is This Useful?

The Query Settings panel acts like a **history log** of your data cleaning process. It’s helpful for:

* Undoing mistakes
    
* Documenting your steps
    
* Ensuring consistency and repeatability
    
* Debugging broken queries
    

### 🧠 Pro Tip:

If the **Query Settings pane** is missing, go to the **View tab** and make sure the **Query Settings** checkbox is ticked ✅.

---

## **2 Formula Bar**

### ✍️ Power Query Editor: Understanding the **Formula Bar**

One of the most powerful tools in Power BI’s **Power Query Editor** is the **Formula Bar** — yet it's often overlooked by beginners. This simple-looking input field holds the key to understanding and customizing the transformations you're applying to your data.

### 🔍 What is the Formula Bar?

The **Formula Bar** displays the **M code** (short for Power Query Formula Language) that Power BI uses behind the scenes for each transformation step.

### 🧠 Why is it called **M Code**?

The name **"M"** in **M Code** stands for **"Mashup"** — because it was originally designed as the **Mashup language** used in Microsoft’s data integration tools to **"mash up"** data from multiple sources.

In your screenshot, it shows this formula:

```plaintext
=Table.TransformColumnTypes(#"Expanded Table Column1",{{"Source.Name", type text}, {"Task Name", type text}})
```

This line tells Power BI to **convert the "**[**Source.Name**](http://Source.Name)**" and "Task Name" columns into text type** — a transformation applied during the "Changed Type" step.

### ✅ Key Features:

* ✏️ **View and edit transformation steps** in raw M code.
    
* 🛠️ Allows you to **customize or fine-tune** Power BI’s automatic transformations.
    
* 🔄 Enables better control, especially when modifying logic that isn't easily handled through the ribbon UI.
    
* 🧠 Great for **learning M code** and developing advanced queries.
    
    ### 🧠 Why It's Useful for You
    
* You can quickly correct or optimize a transformation.
    
* Helpful for copying steps to reuse in another query.
    
* Lets you **understand exactly what Power BI is doing** behind the scenes.
    
* Ideal when working with complex steps like **merging**, **expanding records**, or **conditional logic**.
    

### 💡 Pro Tip:

Use the **Advanced Editor** (next to the formula bar in the ribbon) when you want to see or modify the **entire query script** at once.

## 3 Monospaced

### 🖋️ Power Query Editor: What Does the **Monospaced** Option Do?

Inside the **View tab** of Power Query Editor, there’s a small but useful checkbox labeled **"Monospaced"**. While it may look like a simple font setting, it plays a helpful role when reading or editing code in the Formula Bar or Advanced Editor.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754622855969/7570f8cf-fb79-496b-97bc-55bc8001b203.png align="center")

### 🔤 What is a Monospaced Font?

A **monospaced font** (also called a **fixed-width font**) means **every character takes up the same amount of space** — unlike regular fonts where an “i” is narrower than a “w”.

Examples of monospaced fonts:

* Courier New
    
* Consolas
    
* Lucida Console
    

### Before

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754622956494/d63df076-174d-4cec-8a5b-0d156ce41737.png align="center")

### After

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754623000448/98457ba8-bfc6-4270-8eb1-b7814037906f.png align="center")

### ✅ What Happens When You Enable "Monospaced"?

* It changes the **Formula Bar text** to a monospaced font.
    
* This makes the **M code easier to read and align** — especially for:
    
    * Indentation
        
    * Nested functions
        
    * Multi-line expressions
        
    * Editing complex transformations
        

### 🧠 Why Use It?

| Without Monospaced | With Monospaced |
| --- | --- |
| Harder to align or compare code visually | Easy to see structure and spacing |
| Less coding comfort | Familiar coding experience for developers |
| May introduce accidental mistakes in long code | Helps maintain clean and readable format |

## **4 Show Whitespace**

### 🧾 Power Query Editor: What Does the **Show Whitespace** Option Do?

When you're editing or reviewing M code in Power BI's Power Query Editor, formatting can make a big difference. The **"Show Whitespace"** option helps you see **hidden formatting characters** such as spaces, tabs, and line breaks.

### 🧱 What is Whitespace?

Whitespace refers to **invisible characters** like:

* **Spaces**
    
* **Tabs**
    
* **New lines**
    

These characters don’t appear by default, but they can **impact how your code is read or copied**, especially in:

* Multi-line logic
    
* Indented transformations
    
* Pasted code from external sources
    
* ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754623497085/ede89394-008c-47b7-b196-4a2535056d97.png align="center")
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754623529969/6f7cbddb-c596-48e8-9260-7048192e4451.png align="center")
    
    ✅ What Happens When You Check “Show Whitespace”?
    
* It **reveals hidden characters** like spaces (·) and tabs (→) inside the **Formula Bar** or **Advanced Editor**.
    
* Helps you detect:
    
    * Unintentional spaces
        
    * Misaligned tabs
        
    * Extra new lines or spacing errors
        

### 🧠 Pro Tip:

Combine **Show Whitespace** with **Monospaced font** for a cleaner, developer-friendly editing experience in Power Query.

## **5 Column Quality**

### ✅ Power Query Editor: What Is **Column Quality** and Why Is It Useful?

When working with real-world datasets, data quality issues like **null values** or **errors** are common. The **Column Quality** feature in Power BI's **Power Query Editor** helps you **detect and understand these issues visually** before loading data into your model.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754627255698/1dfd4e94-5351-4083-82e0-f0b4c586adff.png align="center")

### 🧪 What Does "Column Quality" Show?

When enabled, it displays a **small bar chart** directly beneath each column in the data preview, summarizing:

* ✅ **Valid values** (green) – usable data
    
* ⚠️ **Errors** (red) – rows that caused an error during transformation
    
* ⬜ **Empty** (gray) – null or missing values🧠 Why Use Column Quality?
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754628017112/5aad78ed-7f61-4fd2-ac0e-1a16b036ac9d.png align="center")

### 📌 Column 1 (Name)

* ✅ **Valid: 82%**
    
* ⚫ **Empty: 18%**
    
* 🔴 **Error: 0%**
    

✔ This means:

* 9 out of 11 values are valid text entries
    
* 2 are empty (null or blank)
    
* No transformation errors occurred
    

---

### 📌 Column 2 (Age — Numeric Type)

* 🔴 **Error: 18%**
    
* ✅ **Valid: - %**
    
* ⚫ **Empty: - %**
    

❗ This means:

* You've **converted this column to numeric** (`123` icon).
    
* Some values, like `"twenty-five"` or `"Error"`, cannot be parsed as numbers ➡ **Power Query marks them as errors**.
    
* Because of these errors, **Power BI can't determine how many are valid or empty**, so those percentages are shown as **dashes (- %)**.
    

> 🧠 Power BI doesn’t show Valid/Empty stats when **errors prevent accurate calculation**.

### 📌 Column 3 (Email)

* ✅ **Valid: 91%**
    
* ⚫ **Empty: 9%**
    
* 🔴 **Error: 0%**
    

✔ Interpretation:

* 10 values are valid text strings (even if the email format is questionable)
    
* 1 is blank or null
    
* No error has been caused yet, because no transformation or validation has been applied on email format
    

---

## 🧠 Key Takeaways

| Concept | Meaning |
| --- | --- |
| `Valid` | Value type matches the expected data type (e.g., number, text) |
| `Error` | A transformation (e.g., data type change) caused an invalid value |
| `Empty` | Null, blank, or missing entry |
| `- %` (dash) | Cannot calculate due to presence of errors |

### 💡 Pro Tip:

Use **Column Quality** along with:

* **Column Profile** (for deeper stats)
    
* **Column Distribution** (for frequency/count insights)
    

## **6 Column Distribution**

### 📊 Power Query Editor: What Is **Column Distribution** and How Does It Help?

One of the most powerful tools for **exploring your data at a glance** in Power BI’s Power Query Editor is the **Column Distribution** feature. It helps you **visually understand the spread of values** in each column — before you even start analyzing.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754628852953/13581489-b584-44cd-932d-004eaaa46a15.png align="center")

### 📌 What Does "Column Distribution" Do?

When enabled, this option shows a **horizontal bar** under each column with:

* **A count of distinct values**
    
* **A count of unique values**
    
* **A mini histogram** that gives a **quick visual preview** of how values are distributed in that column
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754629231122/e55ca37b-aec8-4ace-8f53-75c3f7dc349f.png align="center")

### 📘 [**Source.Name**](http://Source.Name)

* `2 distinct, 0 unique`
    

✅ **Meaning**:

* Only **2 different values** exist (likely just 2 Excel files used as source).
    
* But **none of them appear only once** → i.e., **every value is repeated**.
    
* **That's why: 0 unique**.
    

### 📘 **Task Name**

* `990 distinct, 983 unique`
    

✅ **Meaning**:

* There are **990 different task names** overall.
    
* Out of those, **983 appear only once** (unique).
    
* So, **7 task names are repeated**.
    

💡 **Use case**:

* You can use this to identify **repeated tasks or duplicates**.
    
* 🧠 What Insights Can You Get?
    

| Insight | Example |
| --- | --- |
| Are there duplicates? | Low unique count = possible duplicates |
| Are values evenly spread? | Histogram bar shows frequency |
| Are values consistent? | One dominant value = skewed data |
| Is the column worth analyzing? | High uniqueness = good candidate for grouping, filtering, etc. |

---

## **7 Column Profile**

### 🔍 Power Query Editor: Understanding the **Column Profile** (with Real Example)

Power BI's **Power Query Editor** includes several powerful profiling tools that help you inspect your data before you clean or transform it. One of the most informative among them is the **Column Profile** feature.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754629704486/ba57706a-8aa4-41ca-af0d-db8389a14a92.png align="center")

### 📌 What Is Column Profile?

**Column Profile** provides a **detailed statistical summary** of any column you select. It appears **at the bottom** of the Power Query window once enabled.

### 🧪 Real Example: "Bucket Name" Column

In the screenshot, we selected the **“Bucket Name”** column, which contains support categories like:

* Mobile / SIM Connectivity Issues
    
* OCS Related Issues
    
* ERP/CRM/Web Application Issues
    
* Windows AD Users /Email Issues
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754629791122/70337b17-dfe7-4b37-bb1e-08b1acea2cf8.png align="center")

### 🧾 What You See in Column Profile

#### 1️⃣ **Column Statistics (Left Panel)**

| Metric | Value | What It Tells Us |
| --- | --- | --- |
| Count | 1000 | Total rows in the column |
| Error | 0 | No transformation or data type errors |
| Empty | 0 | No null or missing values |
| Distinct | 29 | 29 different category names exist |
| Unique | 1 | Only one value appears **once** |
| Empty string | 0 | No values are blank strings (“”) |
| Min / Max | A–Z | Alphabetical range of the values |

💡 **Insight**: While there are 29 categories, only **1 appears only once** — suggesting that most values are repeated.

#### 2️⃣ **Value Distribution (Right Panel)**

This section gives a **visual histogram** showing how frequently each category appears:

* The most common is **"Mobile / SIM Connectivity Issues"**
    
* Others like **"OCS Related Issues"**, **"Windows AD Users"**, and **"ERP/CRM Issues"** also occur frequently
    
* Smaller bars indicate rarer categories (e.g., Billing issues, Ownership transfer, etc.)
    

📊 This helps spot:

* **Dominant categories**
    
* **Long-tail items**
    
* **Data imbalance**
    

### ✅ Why Use Column Profile?

| Benefit | Description |
| --- | --- |
| 🔍 Detect issues early | Spot missing, inconsistent, or unexpected values |
| 📉 Understand distributions | Visualize how your data is spread |
| 🧼 Plan better transformations | Focus on cleaning the right areas |
| 📋 Validate data types | Confirm no type mismatches or formatting errors |

### 💡 Pro Tip:

Combine **Column Profile** with:

* ✅ **Column Distribution** (for distinct vs unique count)
    
* ✅ **Column Quality** (for valid, error, empty percentage)
    

## **8 Go to Column**

### Power Query Editor: What is **Go to Column**?

When working with wide tables that contain **dozens or even hundreds of columns**, it can be tedious to scroll horizontally just to find the one you want. That’s where the **“Go to Column”** feature comes in — a **quick navigation tool** in Power BI’s Power Query Editor.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754632259291/716edff5-771a-47ca-9fb0-eac34b9f3078.png align="center")

### 📌✨ What Does It Do?

When you click **Go to Column**, a pop-up appears showing a **list of all columns** in the current table.

You can:

* 🔍 **Search** by column name
    
* ✅ **Select a column** from the list
    
* 📍 Click **OK** to jump directly to that column
    

### 🎯 Why It’s Useful

| Scenario | How “Go to Column” Helps |
| --- | --- |
| Working with wide tables | Jump to the needed column instantly without scrolling |
| Exploring new data | Quickly scan all available column names |
| Debugging or transforming | Navigate straight to a problem column (e.g., with errors) |
| Applying filters or renames | Find and select columns faster in large datasets |

---

## **9 Always Allow**

### 🔐 Power Query Editor: What Does the **“Always Allow”** Option Do?

While working in Power Query, especially with external files, web sources, or dynamic content like parameters and functions, you may encounter a **“Permission Required”** prompt asking you to approve access each time. The **“Always allow”** checkbox helps streamline that process.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754632586031/67e06d23-075d-4226-8e21-307555df5a76.png align="center")

### 🧭 What It Does

When **enabled**, the **“Always allow”** option:

* Automatically grants permission to evaluate **preview queries** for things like:
    
    * **Parameters**
        
    * **Custom functions**
        
    * **Dynamic file paths**
        
* Reduces the number of prompts asking if you're okay to run them
    

### 🎯 Why Use It?

| Scenario | Benefit |
| --- | --- |
| You use **parameter-driven queries** | Prevents repeat permission prompts every time you apply changes |
| You connect to **external files or APIs** | Allows smooth refreshing and previewing |
| You're developing multiple queries using **functions** | Avoids constant confirmation interruptions |

### 💡 Pro Tip:

If Power BI prompts you too often while developing parameterized reports or using custom functions, enable **“Always allow”** temporarily, then disable it before publishing.

## **10 Advanced Editor**

### 🧠 Power Query Editor: What Is the **Advanced Editor**?

If you're ready to go beyond the visual interface and directly manipulate the logic behind your transformations, the **Advanced Editor** is your secret weapon. It's where you can view and edit the **M code** (Power Query Formula Language) that powers your query steps.

---

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754632996545/60b171e8-7bc9-431f-b17a-9ddfaec00330.png align="center")

### 🛠️ What Can You Do in the Advanced Editor?

* ✍️ **View the full M code** generated by your transformations
    
* 🧾 **Modify or write custom queries** manually
    
* 📑 **Copy/paste** queries between files or projects
    
* 🧩 Create **dynamic queries** using variables and parameters
    
* 🐞 **Debug errors** by analyzing step-by-step M logic
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754633110838/c09208bb-33cb-4919-8bed-8dc81976cd31.png align="center")

### 🔤 Example: A Simple M Code

```plaintext
let
    Source = Excel.Workbook(File.Contents("C:\Data\Sales.xlsx")),
    SalesData = Source{[Name="Sales"]}[Content],
    ChangedType = Table.TransformColumnTypes(SalesData,{{"Amount", type number}})
in
    ChangedType
```

This query:

* Loads data from an Excel file
    
* Selects the **Sales** worksheet
    
* Changes the **Amount** column to numeric
    

---

### 🔒 Why Use Advanced Editor?

| Use Case | Benefit |
| --- | --- |
| Complex transformations | More control and flexibility |
| Copying steps between reports | Reusable, portable code |
| Performance tuning | Optimize query logic |
| Learning M language | Great for deeper Power BI skills |

---

### ⚠️ Tips for Beginners

* Don’t worry if it looks scary — Power BI writes this code for you.
    
* Start by **reading** the M code of existing transformations.
    
* Use the **Formula Bar** for small changes, and Advanced Editor for full overview.
    

## 11 Query dependencies

### 🔗 Power BI Query Dependencies – Understand Your Data Flow at a Glance

In Power BI's Power Query Editor, the **Query Dependencies** view is like your **data map**. It helps you see **how different queries are connected**, where the data flows from, and which tables depend on which others.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754634392032/e8150322-caa9-4c0b-850c-974d98872627.png align="center")

### 📘 Use Case: Sales Performance Reporting

Suppose you're building a sales report based on quarterly sales data and regional targets. You’ve structured your queries like this:

| Query Name | Purpose |
| --- | --- |
| `Sales_Q1` | Raw sales data for Quarter 1 |
| `Sales_Q2` | Raw sales data for Quarter 2 |
| `All_Sales` | Combined Q1 + Q2 data |
| `Region_Targets` | Monthly sales targets per region |
| `Sales_vs_Target` | Final output comparing actual sales vs. target |

### 🔍 What is Query Dependencies?

The **Query Dependencies view** provides a **visual representation** of how your queries are related.

You can access it via:

📍 `View` tab ➜ `Query Dependencies`

---

### 📊 Diagram Example

Here’s how the dependencies appear for our sales project:

```plaintext
Sales_Q1       Sales_Q2
   \             /
    \           /
     \         /
     →   All_Sales   ← Region_Targets
                \
                 → Sales_vs_Target
```

This view tells us:

* `All_Sales` is built from **Sales\_Q1 + Sales\_Q2**
    
* `Sales_vs_Target` is built from **All\_Sales + Region\_Targets**
    
* `Query1` (if seen separately) is not connected — possibly unused or for staging
    

---

## 🎯 Why is Query Dependencies Useful?

* ✅ **Track Data Lineage**  
    See exactly where your final report values are coming from.
    
* 🪛 **Troubleshoot Quickly**  
    If a value is wrong, trace back through the query chain to find the root cause.
    
* 🧹 **Clean Unused Queries**  
    Spot disconnected queries that aren't needed and safely remove them.
    
* 🚦 **Optimize Performance**  
    Understand how transformations cascade and avoid unnecessary recalculations.
    

---

💡 **Final Thought:**  
As your report grows complex, **Query Dependencies** becomes your **navigation compass**. Whether you’re building staging tables, merging sources, or building a final dashboard — it’s always worth checking your data flow map.

# Tools

## 1 Diagnose Step

### 🛠 Power Query Diagnostics – Track Performance Step by Step

As your Power BI transformations grow in complexity, so does the **need to monitor performance**. That’s where the **Diagnostics tools in the Tools tab** come into play.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754638521631/d00e8876-85df-480d-bfb1-e47c0dae4a8b.png align="center")

---

### ⚙️ What Does “Diagnose Step” Do?

The **Diagnose Step** feature measures how much time a specific step in your query takes — and **how much of that time is spent on external sources or downstream dependencies**.

💡 This is particularly useful when you're not sure:

* Which transformation is slowing you down
    
* Whether slowness comes from your data source or your logic
    
* If you're over-using merge/join/custom functions
    

---

## 🧪 How to Use It

### Step-by-step:

1. Open Power Query and go to the **Tools** tab.
    
2. Click **Start Diagnostics**.
    
3. Perform the actions or refresh the steps you want to diagnose.
    
4. Click **Stop Diagnostics**.
    
5. You’ll now see **diagnostics tables** automatically created.
    

Alternatively, for more control, use **Diagnose Step** to focus on **only one specific transformation step**.

---

## 📊 What Output Do You Get?

After diagnosing, Power BI gives you two tables:

| Table | Purpose |
| --- | --- |
| 🧱 **Diagnostics\_Partitions** | Shows the total and exclusive duration of each query partition |
| 🧪 **Diagnostics\_Detailed** | Breaks down step-by-step query execution, source type, rows processed, and time taken |

These tables help you answer:

* Which step took the longest?
    
* Was it the actual transformation or a data source delay?
    
* Is my data source (e.g., Excel, SQL, Web) slow?
    

---

## 🕵️ Pro Tips for Interpreting Results

* **High Exclusive Duration (%)** = That step is your main bottleneck
    
* **Low Exclusive but High Total** = The problem is further downstream
    
* **Web or Excel source with high duration** = Try optimizing or replacing the source
    
* **Custom column with long duration** = Consider rewriting logic or using native functions
    

---

## 🧹 Clean Up

To exit or reset diagnostics:

* Use **Cancel Diagnostics** if you no longer want to trace the step
    
* Delete diagnostics tables if not needed for long-term tracking
    

---

## 📌 When to Use This

* Power BI reports are **slow to refresh**
    
* Query performance is **getting worse with more data**
    
* You're dealing with **multiple merged queries**
    
* You want to prove to your team where time is spent
    

---

## ✍️ Final Thoughts

Diagnosing performance in Power Query used to feel like guesswork — now, with **Diagnose Step**, it's a science.

Use this tool as part of your **Power BI performance optimization workflow**, and you’ll not only speed up your reports, but also learn to write cleaner, faster queries.

## **2 Start/Stop Diagnostics**

### 🔍 Power Query Performance Tuning with **Session Diagnostics**

In Power BI, slow refreshes and laggy data loading can frustrate even the most experienced analysts. Thankfully, **Power Query's Diagnostics Tools** give us a way to inspect what’s really going on — especially through **Session Diagnostics**.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754640496513/58581bd8-41a2-4a8a-bd73-4d2c6cbe2d4b.png align="center")

## 🧪 What Is Session Diagnostics?

Unlike **Diagnose Step** (which looks at one step), **Session Diagnostics** captures the **entire refresh session**, tracking every step you perform **from start to finish**.

It gives a full picture of what Power Query is doing behind the scenes:

* Data source access times
    
* Time spent on transformations
    
* Resource usage
    
* Number of rows processed
    
* Query execution sequence
    
    ### 🧰 How to Use Session Diagnostics
    

### Step-by-Step:

1. Go to the **Tools tab** ➜ Click **Start Diagnostics**
    
2. Perform your refresh or query steps (you can add new steps, filter, sort, or apply transformations)
    
3. Click **Stop Diagnostics** when done
    
4. Power BI will create **two new tables** in your Queries pane:
    
    * `Diagnostics_Partitions_...`
        
    * `Diagnostics_Detailed_...`
        

## 📊 What Do the Tables Show?

### 🧱 `Diagnostics_Partitions`

Shows the **partition-level breakdown** — think of this as the “summary” view.

| Column | Meaning |
| --- | --- |
| **Partition Key** | Which query step or source |
| **Start/End Time** | Timestamps of execution |
| **Duration** | Total time taken |
| **Exclusive Duration** | Time taken only by this part (excluding child steps) |

### 🔬 `Diagnostics_Detailed`

Gives you a **step-by-step analysis** of every operation.

| Column | Description |
| --- | --- |
| **Step** | Name of the step |
| **Category** | Source / Transformation / Evaluation |
| **Row Count** | Number of rows processed |
| **Data Source Kind** | e.g., Excel, SQL, Web |
| **Exclusive Duration (%)** | Bottleneck indicator |
| **Path** | The sequence of step execution |

---

## 🧠 How to Interpret Results

* 🟥 **High exclusive duration = bottleneck**
    
* 🟨 **High row count = might need optimization**
    
* 🟦 **Source queries slow? Try reducing data or filtering early**
    
* 🟩 **Nested joins or custom columns slow? Replace with native transformations**
    

---

## ✅ Use Cases

| Scenario | Use Diagnostics |
| --- | --- |
| Refresh taking too long | ✔️ Identify which query or source is slow |
| Merged queries feel heavy | ✔️ Spot joins with high durations |
| Curious how transformations flow | ✔️ Understand the execution path |

---

## 💡 Bonus Tips

* Delete the diagnostics tables when done (to avoid clutter)
    
* You can compare different sessions side-by-side
    
* Combine with **Query Dependencies** for a full visual map of your model
    

---

## ✍️ Final Thoughts

**Session Diagnostics** is your Power BI X-ray machine.

Instead of guessing why your report is slow, use diagnostics to **see the exact steps**, **analyze durations**, and **optimize intelligently**.

By leveraging this tool, you gain visibility into Power Query’s engine and can confidently **build faster, more efficient reports.**

## 3 Diagnostic Options

### ⚙️ Power BI Diagnostic Options – Fine-Tune What You Trace

As part of Power Query’s powerful **diagnostic toolkit**, the **Diagnostic Options** button gives you **granular control** over what Power BI captures during a **Session Diagnostics** run.

If you've ever wanted to **reduce clutter** or focus only on **specific performance bottlenecks**, this is where you configure your tracing behavior.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754640997668/12c61bf6-f738-48b9-8671-ad7d498b7498.png align="center")

---

## 🧰 What Is It For?

When you click **Diagnostic Options**, Power BI opens a settings window where you can:

* ✅ Enable or disable **detailed traces**
    
* 🎯 Focus on **specific categories** like:
    
    * Evaluation steps
        
    * Cache hits
        
    * Background refresh
        
    * Diagnostics related to specific **data sources**
        
* 📉 Reduce the **amount of captured data** if you only want the essentials
    

---

## ✨ Why Use Diagnostic Options?

| Use Case | Why It Helps |
| --- | --- |
| You only care about **slow queries** | Exclude unnecessary trace categories |
| Your diagnostics table is too large | Disable low-priority events |
| You're troubleshooting a specific **data source** | Filter to focus only on that connector |

## 🧪 Tip for Power Users

When running diagnostics on **large models**, the default settings can generate huge logs.

To stay efficient:

> ✅ Use **Diagnostic Options** to reduce noise  
> 🔍 Focus on **transformation steps**, **refresh durations**, or **custom connectors**

---

## 🔚 Wrapping It All Up

The **Diagnostic Options** panel is like your filter lens. It helps you:

* **Target the root cause** more effectively
    
* **Reduce distractions** from irrelevant trace data
    
* **Control performance impact** during diagnostics
    

When used in combination with:

* **Start/Stop Diagnostics**
    
* **Query Dependencies**
    
* **Diagnose Step**
    

👉 It gives you a **complete control center** for performance tuning in Power BI.

# Help

## 1 Guided Learning

### 🎓 Power BI Guided Learning – Your Built-in Learning Path

When starting with Power BI, it’s easy to feel overwhelmed by all the features, menus, and tools. That’s why Microsoft includes **Guided Learning** right inside Power BI Desktop — a direct link to a **structured, official learning resource** that takes you step-by-step from beginner to confident report builder.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754723656130/bdebe892-08ce-4867-ab74-704492e2ec26.png align="center")

---

### 📌 What is Guided Learning?

The **Guided Learning** button in the **Help** tab is a shortcut to Microsoft’s **Power BI Learning Path** on their official website. This path is broken into clear, progressive lessons, designed for self-paced learning.

[https://learn.microsoft.com/en-gb/power-bi/fundamentals/desktop-getting-started](https://learn.microsoft.com/en-gb/power-bi/fundamentals/desktop-getting-started)

### 🧭 What’s Inside Guided Learning?

The learning path covers:

* **Getting Started with Power BI**  
    Understanding the purpose of Power BI and how it works in business intelligence.
    
* **Connecting to Data**  
    Step-by-step tutorials on importing data from Excel, SQL Server, the web, and other sources.
    
* **Transforming Data**  
    Learn how to clean, reshape, and prepare data using **Power Query** before building visuals.
    
* **Data Modeling**  
    Create relationships, calculated columns, and measures for better analysis.
    
* **Creating Reports & Dashboards**  
    Build interactive visuals and design engaging dashboards.
    
* **Publishing & Sharing**  
    Share your work securely through the Power BI Service.
    

---

### ✅ Why Use Guided Learning?

* **Structured & Beginner-Friendly** – Ideal for those new to Power BI.
    
* **Official & Up-to-Date** – Content is maintained by Microsoft.
    
* **Free** – No subscription required to access learning materials.
    
* **Self-Paced** – Learn when and where you want.
    

💡 **Tip:** Even experienced users can use Guided Learning to explore **new features** or **refresh core skills**. It’s more than a beginner’s tool — it’s a reference you can revisit anytime.

## 2 Documentation

### 📚 Power BI Documentation – Your Complete Technical Guide

When working in Power BI, there’s often a moment where you think:

> *"I wish I had a detailed explanation of this feature."*

That’s exactly where the **Documentation** button in the **Help** tab comes to the rescue.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754723981607/8bc3240d-4bef-4b1d-9817-ce10c091af5a.png align="center")

### 📌 What is the Documentation Option?

The **Documentation** button is a quick link to the **official Microsoft Power BI documentation site**. It provides detailed, authoritative guidance on **every tool, feature, and function** in Power BI.

### 🧭 What You’ll Find in the Documentation

The site includes:

* **Getting Started Guides**  
    Learn the basics of installing and using Power BI Desktop.
    
* **Connecting to Data Sources**  
    Instructions for importing data from Excel, SQL Server, SharePoint, APIs, and more.
    
* **Power Query Transformation Guides**  
    Detailed steps for cleaning and reshaping data.
    
* **Data Modeling & DAX Reference**  
    Learn how to create relationships, measures, calculated columns, and master DAX formulas.
    
* **Visualization Guides**  
    Best practices for designing reports, customizing visuals, and telling data stories.
    
* **Publishing & Collaboration**  
    How to share your reports securely through the Power BI Service.
    
* **Admin & Governance**  
    Manage security, compliance, and organizational settings.
    

### ✅ Why Use the Documentation?

* **Official & Accurate** – Maintained by Microsoft’s product team.
    
* **Searchable** – Quickly find step-by-step instructions.
    
* **Always Updated** – Reflects the latest features and changes.
    
* **Great for All Levels** – Useful for both beginners and advanced users.
    
    💡 **Pro Tip:** Bookmark the **Power BI Documentation** site — it’s an invaluable reference you’ll use often, especially when troubleshooting or exploring advanced features.
    

## 3 Training Videos

### 🎥 Power BI Training Videos – Learn by Watching

Sometimes reading through guides isn’t enough — you need to see **how things are done** in action. That’s exactly why Microsoft includes **Training Videos** in the **Help** tab of Power BI Desktop.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754724197140/61be9d8d-befc-42f4-86e8-af05a49fb0a8.png align="center")

### 📌 What is the Training Videos Option?

The **Training Videos** button opens Microsoft’s **official Power BI video library** in your browser. These videos provide **visual, step-by-step demonstrations** of key Power BI features, making it easier to follow along and learn.

### 🧭 What You’ll Find in the Training Videos

The video library includes:

* **Getting Started Tutorials**  
    Learn the basics of connecting to data, creating visuals, and publishing reports.
    
* **Data Preparation**  
    Step-by-step videos on using **Power Query** to clean and transform data.
    
* **Data Modeling**  
    How to set up relationships, use DAX, and design effective data models.
    
* **Visualizations & Report Design**  
    Best practices for creating interactive charts, maps, tables, and dashboards.
    
* **Advanced Features**  
    Tips on parameters, bookmarks, drillthrough, and custom visuals.
    
* **Collaboration & Sharing**  
    Learn how to share reports via the Power BI Service and collaborate with others.
    

---

### ✅ Why Use Training Videos?

* **Learn Visually** – See each step in action for better understanding.
    
* **Official & Up-to-Date** – Created by Microsoft’s Power BI team.
    
* **Beginner to Advanced** – Suitable for all skill levels.
    
* **Self-Paced** – Watch anytime and replay as needed.
    

---

tutorials💡 **Pro Tip:** Keep a second monitor (or split screen) open so you can **follow along in Power BI Desktop** while watching the training videos. This hands-on approach helps you learn faster.

## 4 Support

### ❓ Power BI Support – Get Help When You Need It

Even experienced Power BI users sometimes face technical issues, unexpected errors, or questions about best practices. The **Support** option in the **Help** tab is your direct link to Microsoft’s official assistance channels.

[https://support.fabric.microsoft.com/support/](https://support.fabric.microsoft.com/support/)

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754724578800/dd9fde22-5c9a-4559-b9e2-b339fdf42d68.png align="center")

### 📌 What is the Support Option?

Clicking **Support** in the Help tab opens Microsoft’s **Power BI Support page** in your browser. From here, you can:

* Search the knowledge base for solutions to common issues.
    
* Access troubleshooting guides for errors and performance problems.
    
* Open a **support ticket** with Microsoft’s technical team.
    

### 🧭 What You’ll Find in the Support Page

The Power BI Support hub provides:

* **Troubleshooting Articles**  
    Step-by-step solutions for known errors and feature issues.
    
* **Service Status Updates**  
    Check if an outage or maintenance is affecting Power BI services.
    
* **Community & Forums**  
    Post questions and get answers from other Power BI professionals.
    
* **Contact Microsoft Support**  
    If you have a paid Power BI subscription, you can log a support ticket for one-on-one help.
    

### ✅ Why Use Power BI Support?

* **Fast Problem Resolution** – Find official fixes or workarounds.
    
* **Up-to-Date Information** – Stay informed about outages or known issues.
    
* **Access to Experts** – Connect with Microsoft engineers for complex problems.
    
* **Community Input** – Learn from solutions other users have already tried.
    

💡 **Pro Tip:** Always check the **Power BI Service Status** before spending time troubleshooting — sometimes the issue is due to a temporary service outage.

## 5 About

### ℹ️ Power BI About – Version & Information Hub

Knowing exactly which version of Power BI Desktop you’re using is more important than it might seem — especially when troubleshooting issues or checking feature compatibility. The **About** option in the **Help** tab gives you all this information in one place.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754724827289/45e0b5e6-ef30-43b1-8f81-be2f47ab457e.png align="center")

### 📌 What is the About Option?

The **About** button opens a dialog box with key information about your **Power BI Desktop installation**, including:

* **Version Number** – Helps you confirm if you have the latest release.
    
* **Build Number** – Useful when reporting bugs or issues to Microsoft.
    
* **License Information** – Shows your license type and terms.
    
* **Copyright & Legal Details** – Microsoft’s usage rights and policies.
    

### 🧭 Why the About Section Matters

* **Troubleshooting**  
    When contacting support or searching the documentation, version numbers help ensure you’re looking at the right instructions.
    
* **Feature Availability**  
    Some new Power BI features are only available in recent updates. Checking your version tells you if you need to update.
    
* **Security & Stability**  
    Running the latest version ensures you benefit from the newest security fixes and performance improvements.
    

---

### ✅ Benefits of Using the About Option

* Quick access to version & build details.
    
* Essential for technical support requests.
    
* Ensures you’re aware of update needs.
    

---

💡 **Pro Tip:** Make it a habit to check the **About** section after installing an update — that way, you can confirm you’re running the latest build.

## 6 Power BI Blog

### 📰 Power BI Blog – Stay Updated with the Latest from Microsoft

Power BI is constantly evolving, with **new features, updates, and best practices** released almost every month. The **Power BI Blog** in the **Help** tab is your direct gateway to staying informed and ahead of the curve.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754725166424/5fd7398b-2eb0-447b-b7cc-7cdbb4a66604.png align="center")

### 📌 What is the Power BI Blog Option?

The **Power BI Blog** button opens Microsoft’s **official Power BI blog** in your browser. This blog is maintained by the Microsoft Power BI team and includes:

* Monthly feature summaries.
    
* Announcements of new tools and updates.
    
* Real-world use cases and success stories.
    
* Tips, tricks, and how-to guides from Power BI experts.
    

---

### 🧭 What You’ll Find in the Power BI Blog

* **Monthly Feature Updates**  
    Detailed breakdown of the latest Power BI Desktop and Service updates.
    
* **New Feature Announcements**  
    Learn about upcoming capabilities before they’re widely rolled out.
    
* **Tutorials & Tips**  
    Step-by-step guidance to make the most of new and existing features.
    
* **Community Highlights**  
    Showcases dashboards, reports, and creative uses of Power BI from around the world.
    

---

### ✅ Why Visit the Power BI Blog?

* **Stay Current** – Be the first to know about new features.
    
* **Learn Best Practices** – Direct from Microsoft and the Power BI community.
    
* **Find Inspiration** – See how other users are building impactful reports.
    
* **Plan Ahead** – Prepare for features in preview or on the roadmap.
    

---

### 🚀 How to Access It in Power BI Desktop

🌐 https://powerbi.microsoft.com/blog/

💡 **Pro Tip:** Bookmark the blog and check it at the start of every month — that’s when Microsoft typically posts the **Power BI Desktop Monthly Update**.

## 7 Community

### 👥 Power BI Community – Learn, Share, and Collaborate

Sometimes the fastest way to solve a problem or discover a new trick isn’t through official documentation — it’s by connecting with people who’ve been there before. That’s where the **Power BI Community** comes in.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754730126170/0a46cf06-2d4d-4684-aa15-57d01f8d827a.png align="center")

[https://community.fabric.microsoft.com/t5/Power-BI-forums/ct-p/powerbi](https://community.fabric.microsoft.com/t5/Power-BI-forums/ct-p/powerbi)

### 📌 What is the Community Option?

The **Community** button in the **Help** tab opens Microsoft’s **official Power BI Community site**, a hub where Power BI users from around the world share knowledge, ask questions, and collaborate.

### 🧭 What You’ll Find in the Power BI Community

* **Discussion Forums**  
    Post questions, get answers, or help others with their Power BI challenges.
    
* **Knowledge Base Articles**  
    Community-created solutions and how-to guides.
    
* **Events & Webinars**  
    Join live or recorded sessions to learn from experts and peers.
    
* **Showcase & Inspiration**  
    View creative dashboards, reports, and data stories shared by the community.
    
* **User Groups**  
    Connect with Power BI users in your region for networking and collaboration.
    

### ✅ Why Join the Power BI Community?

* **Get Quick Help** – Tap into the knowledge of thousands of experienced users.
    
* **Learn Best Practices** – Discover efficient solutions and workflows.
    
* **Stay Engaged** – Keep up with feature discussions and upcoming changes.
    
* **Give Back** – Share your own insights and help others grow.
    

---

💡 **Pro Tip:** Create a free account in the Power BI Community — it lets you post questions, track responses, and even earn badges for contributions.

## **8 Power BI for Developers**

### **Power BI for Developers – Overview**

The **Power BI for developers** feature in the Help tab is designed for technical users who want to extend Power BI’s capabilities beyond its standard drag-and-drop interface. It provides resources, documentation, and tools that allow developers to:

[https://learn.microsoft.com/en-gb/power-bi/developer/?WT.mc\_id=PBIService\_HelpMenu](https://learn.microsoft.com/en-gb/power-bi/developer/?WT.mc_id=PBIService_HelpMenu)

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754795771819/ac7a500b-1286-44ba-8b89-5ccdd24f3b2f.png align="center")

### **1\. Build Custom Visuals**

* Developers can create **custom visuals** using TypeScript and the Power BI Custom Visuals SDK.
    
* These visuals can be tailored to specific business needs and imported into Power BI reports.
    

### **2\. Embed Power BI in Applications**

* Using **Power BI Embedded** and the **REST APIs**, developers can integrate interactive reports and dashboards into their own applications or websites.
    
* Supports embedding for both internal (organization) and external (customer-facing) users.
    

### **3\. Automate & Manage via APIs**

* The **Power BI REST API** allows automation of:
    
    * Dataset refreshes
        
    * Workspace and report management
        
    * User access and permissions
        
* Useful for large-scale deployments or automated workflows.
    

### **4\. Access Developer Documentation**

* Direct link to the **Microsoft Power BI Developer Center** where you’ll find:
    
    * API references
        
    * Sample code
        
    * Tutorials for embedding and building custom visuals
        
    * GitHub repositories for Power BI development tools
        

---

**💡 When to Use:**  
If you are:

* A **developer** integrating Power BI into your apps.
    
* A **BI professional** who needs custom visuals or automation.
    
* An **IT admin** building scalable Power BI solutions.
    

**🔗 Quick Path in Power BI Desktop:**  
`Help → Power BI for developers` → Opens official developer resources.

## 9 **Samples**

### **Samples in Power BI – Learn by Exploring**

The **Samples** option in Power BI Desktop’s Help tab provides ready-made datasets and reports that you can download and explore. These samples are designed to help you quickly understand Power BI’s features, learn best practices in report building, and experiment without needing your own data.  
[https://learn.microsoft.com/en-gb/power-bi/create-reports/sample-datasets#the-power-bi-samples-as-pbix-files](https://learn.microsoft.com/en-gb/power-bi/create-reports/sample-datasets#the-power-bi-samples-as-pbix-files)

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754796079045/d70b4e9f-4fa4-491d-9a10-569f6f111cfd.png align="center")

### **What You Get in Samples**

* **Pre-built Datasets**  
    Clean, structured data files (Excel, CSV, or .pbix) ready for analysis.
    
* **Example Dashboards & Reports**  
    Fully designed Power BI reports showcasing:
    
    * Data modeling
        
    * Visual design best practices
        
    * Interactive filters and slicers
        
* **Variety of Scenarios**  
    Samples include real-world business cases, such as:
    
    * Retail analysis
        
    * Sales performance
        
    * Human resources analytics
        
    * Financial dashboards
        

### **Benefits of Using Samples**

1. **Learn Faster** – See how professional reports are structured.
    
2. **Practice Skills** – Test Power Query transformations, DAX formulas, and visualization techniques.
    
3. **Inspire Your Designs** – Adapt and customize layouts for your own projects.
    
4. **Safe Environment** – No risk of altering live or sensitive company data.
    

### **How to Access**

1. Go to **Help** tab.
    
2. Click **Samples** under the **Community** section.
    
3. Choose a sample file to download from Microsoft’s official library.
    
4. Open it in Power BI Desktop and explore.
    

**💡 Tip:**  
Use sample data to practice:

* **DAX calculations**
    
* **Custom visuals**
    
* **Page navigation**
    
* **Report themes**
    

## **10 Community Galleries**

### **Community Galleries – A Hub of Shared Power BI Creations**

The **Community Galleries** option in Power BI Desktop connects you to Microsoft’s online community space, where Power BI users from around the world share their reports, dashboards, themes, and custom visuals.

It’s a place to **learn from others, get inspired, and showcase your own work**.

[https://community.fabric.microsoft.com/t5/Galleries/ct-p/PBI\_Comm\_Galleries](https://community.fabric.microsoft.com/t5/Galleries/ct-p/PBI_Comm_Galleries)

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754796336534/00037836-d40b-4a42-9b6d-01827a4566b1.png align="center")

### **What You Can Find**

1. **Report Galleries**  
    Explore reports built by other Power BI users. These often demonstrate:
    
    * Advanced DAX usage
        
    * Creative visual layouts
        
    * Industry-specific analytics
        
2. **Data Stories**  
    Real-world applications of Power BI, where users explain the data challenge they faced, their approach, and the results.
    
3. **Custom Themes**  
    Download professionally designed **JSON theme files** to instantly style your own reports with matching colors and fonts.
    
4. **Custom Visuals**  
    Browse community-created visuals beyond the default Power BI set, adding more variety and interactivity.
    

---

### **Benefits of Using Community Galleries**

* **Learn Best Practices** – See how experts handle design, navigation, and interactivity.
    
* **Save Time** – Download ready-to-use themes and visuals instead of creating from scratch.
    
* **Get Inspiration** – Discover creative approaches to data storytelling.
    
* **Engage with the Community** – Ask questions, leave feedback, or share your own work.
    

---

### **How to Access**

1. In Power BI Desktop, go to the **Help** tab.
    
2. Under the **Community** section, click **Community Galleries**.
    
3. Your browser will open Microsoft’s official Power BI Community Gallery page.
    

---

**💡 Tip:**  
If you find a theme or visual you like, **save it locally** so you can apply it across multiple reports for a consistent brand style.

## **11 Submit an Idea**

### **Submit an Idea – Shape the Future of Power BI**

The **Submit an Idea** option in Power BI Desktop is your direct link to Microsoft’s **Power BI Ideas** platform, where users can propose new features, improvements, or changes they want to see in the product.

It’s a way for the Power BI community to collaborate with Microsoft’s development team and influence the tool’s future roadmap.

[https://community.fabric.microsoft.com/t5/Fabric-Ideas/idb-p/fbc\_ideas](https://community.fabric.microsoft.com/t5/Fabric-Ideas/idb-p/fbc_ideas)

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1754796718715/2c23d598-8dfb-4267-a229-5b04a69cbe95.png align="center")

### **How It Works**

1. **Submit Your Idea**
    
    * Suggest a new feature or enhancement.
        
    * Describe the problem it solves or the improvement it brings.
        
    * Provide relevant examples or use cases.
        
2. **Vote for Ideas**
    
    * Browse through ideas submitted by others.
        
    * Vote for the ones you believe should be prioritized.
        
    * The more votes an idea gets, the more likely it is to attract Microsoft’s attention.
        
3. **Track Progress**
    
    * See whether ideas are under review, planned, or already implemented.
        
    * Follow updates and community discussions around the idea.
        
4. ### **Benefits**
    
5. **Direct Influence** – Your input can help shape Power BI’s features and updates.
    
6. **Community Collaboration** – Engage with fellow users to refine and improve proposals.
    
7. **Transparency** – See how Microsoft responds to community feedback.
    

### **How to Access**

1. Go to the **Help** tab in Power BI Desktop.
    
2. Under the **Community** section, click **Submit an Idea**.
    
3. Your browser will open the official Power BI Ideas website.
    

**💡 Tip:**  
Before submitting, **search existing ideas** to see if yours is already listed — if it is, vote for it instead of creating a duplicate. This increases its visibility and impact.