---
title: "M Language from Scratch in Power Query for Power BI"
datePublished: Sat Oct 11 2025 03:39:20 GMT+0000 (Coordinated Universal Time)
cuid: cmglq806i000002ju6etb4fkv
slug: m-language-from-scratch-in-power-query-for-power-bi

---

## What is Power Query?

Power Query is Power BI’s **data preparation** layer. It lets you **connect**, **clean**, and **reshape** data from Excel, SQL, CSVs, folders, web APIs, and more—**before** analysis. You build steps once, and Power Query repeats them on every refresh.

**Typical tasks**

* Remove/rename columns, fix data types
    
* Filter rows, split/merge columns
    
* Unpivot/pivot, group & aggregate
    
* Merge (join) and append (union) tables
    
* Combine many files from a folder with one reusable pattern
    

## What is the M language?

**M** (for *Mashup*) is the scripting language behind Power Query. Every click you do in the UI is recorded as **M steps** in a `let … in` pipeline. You can read or edit this code in **Advanced Editor** to automate and customize transformations.

**Key traits**

* **Functional**: transformations are functions chained step-by-step.
    
* **Case-sensitive**: `List.Max` ≠ `list.max`. (Correct form is `List.Max`.)
    
* **Strong types**: `type text`, `type number`, `type date`, etc.
    
* **Safe handling**: `try … otherwise` to guard against errors.
    

## Mental model

* A query is a **sequence of steps**; each step returns a table to the next.
    
* Keep **data shaping in Power Query**, do **calculations in DAX** later.
    

## Why use M at all?

* **Repeatability**: one click = one recorded step, replays on refresh.
    
* **Control**: do things the UI can’t (custom functions, dynamic rules).
    
* **Scale**: robust pipelines for folders/monthly files with minimal effort.
    

## Power Query Editor — Quick Start (Hands-on)

## Open the Editor

* In **Power BI Desktop**, go to **Home → Transform data** to open **Power Query** (the data prep window).
    

## Connect to data

* **Home → New Source** → pick your source (Excel, CSV, SQL Server, etc.).
    
* For Excel: choose **Workbook** → select file → pick **Sheet/Table** → **Transform Data**.
    
* (Tip) Rename the query in **Properties** (right pane), e.g., `SampleDataset01`.
    

You can:

* **Reorder/rename/delete** steps (❌ to remove; ⚙ to edit).
    
* Toggle steps to debug transformations.
    

### See the M code

* **Formula Bar** (View → check **Formula bar**) shows M for the **selected step**.
    
* **Home → Advanced Editor** shows the **entire query** (`let … in`) so you can edit or paste code.
    

## Understand “Applied Steps”

Power Query records every action as a step (top-right panel):

**Source** – connection details (provider + file/path).

`= Excel.Workbook(File.Contents("C:\DATA science\Cousera Certifications\Power BI\Complete M Language from Scratch in Power Query for Power BI\Datasets\01. Sample Dataset 01.xlsx"), null, true)`

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1760155622548/54cc4a43-b5db-4d8c-8eb2-f85d4be67da2.png align="center")

**Navigation** – which sheet/table you selected.

`= Source{[Item="Sheet1",Kind="Sheet"]}[Data]`

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1760155729551/8e305b09-6d6d-4870-a486-479702092934.png align="center")

**Promoted Headers** – first row → headers.

`= Table.PromoteHeaders(Sheet1_Sheet, [PromoteAllScalars=true])`

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1760156166350/46021f1b-59b0-4dda-90d2-2632a47038c0.png align="center")

**Changed Type** – auto-detects column data types.

`= Table.TransformColumnTypes(#"Promoted Headers",{{"Product ID", Int64.Type}, {" Product Name", type text}, {" Category", type text}, {" Price", type number}, {" Quantity in Stock", Int64.Type}, {" Discount", type number}, {" Date Added", type text}})`

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1760156039813/e25e0a45-6c32-440f-8ba9-84ff362cd616.png align="center")