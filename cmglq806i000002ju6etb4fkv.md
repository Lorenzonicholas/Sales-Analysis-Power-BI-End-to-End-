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
    

### What is the M language?

**M** (for *Mashup*) is the scripting language behind Power Query. Every click you do in the UI is recorded as **M steps** in a `let … in` pipeline. You can read or edit this code in **Advanced Editor** to automate and customize transformations.

**Key traits**

* **Functional**: transformations are functions chained step-by-step.
    
* **Case-sensitive**: `List.Max` ≠ `list.max`. (Correct form is `List.Max`.)
    
* **Strong types**: `type text`, `type number`, `type date`, etc.
    
* **Safe handling**: `try … otherwise` to guard against errors.
    

### Mental model

* A query is a **sequence of steps**; each step returns a table to the next.
    
* Keep **data shaping in Power Query**, do **calculations in DAX** later.
    

### Why use M at all?

* **Repeatability**: one click = one recorded step, replays on refresh.
    
* **Control**: do things the UI can’t (custom functions, dynamic rules).
    
* **Scale**: robust pipelines for folders/monthly files with minimal effort.
    

## Power Query Editor — Quick Start (Hands-on)

### Open the Editor

* In **Power BI Desktop**, go to **Home → Transform data** to open **Power Query** (the data prep window).
    

### Connect to data

* **Home → New Source** → pick your source (Excel, CSV, SQL Server, etc.).
    
* For Excel: choose **Workbook** → select file → pick **Sheet/Table** → **Transform Data**.
    
* (Tip) Rename the query in **Properties** (right pane), e.g., `SampleDataset01`.
    

You can:

* **Reorder/rename/delete** steps (❌ to remove; ⚙ to edit).
    
* Toggle steps to debug transformations.
    

### See the M code

* **Formula Bar** (View → check **Formula bar**) shows M for the **selected step**.
    
* **Home → Advanced Editor** shows the **entire query** (`let … in`) so you can edit or paste code.
    

### Understand “Applied Steps”

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

## M Language Basics — Variables & Comments (Quick Study Note)

### Where to write M

* **Home → Transform data** → **Advanced Editor** (entire query).
    
* Or use the **Formula bar** to edit the **selected step** (enable via *View → Formula bar*).
    

### 1) The `let … in` pattern

* `let`: define variables/steps.
    
* `in`: return the final expression/value.
    

```plaintext
let
    x   = 10,            // first variable
    y   = 20,            // second variable
    sum = x + y          // last variable → no comma here
in
    sum                   // query returns 30
```

**Rules**

* Put a **comma after every variable** except the last one.
    
* M is **case-sensitive**: `y` ≠ `Y`.
    

```plaintext
let
    y = 20
in
    Y       // Error: different case
```

### 2) Variable names

* Normal identifiers: `TotalSales`, `x1`, `_stage`.
    
* If you need **spaces or special characters**, wrap the name with double quotations and add the **#** symbol:
    

```plaintext
let
    #"My Variable 1" = 10
in
    #"My Variable 1"
```

### 3) Comments

Comments are ignored at runtime and great for documentation.

* **Single-line**: `// comment`
    
* **Multi-line**: `/* comment block */`
    

```plaintext
let
    // Inputs
    x = 10,
    y = 20,

    /* Business rule:
       Use arithmetic sum for demo */
    sum = x + y
in
    sum
```

### 4) Quick troubleshooting

* “**Token Literal expected**”: often a **missing comma** or extra comma after the last variable.
    
* “**Name wasn’t recognized**”: **case mismatch** or identifier not defined.
    
* If the query breaks, delete the last **Applied Step** or open **Advanced Editor** and fix the code.
    

## M Language Data Types — Part 1: **Number**

### What “number” means in M

* `number` is M’s scalar numeric type.  
    It can represent **integers** (e.g., `10`, `-5`) and **decimals** (e.g., `3.14`, `-0.5`).
    
* Column types in tables can be more specific (e.g., `Int64.Type`, `Decimal.Type`, `Double.Type`, `Currency.Type`) but when you work with **scalar** values in code, you’ll usually see plain `number`.
    

```plaintext
let
    v1 = 10,      // integer (number)
    v2 = 3.14,    // decimal (number)
    sum = v1 + v2
in
    sum            // 13.14
```

## Referencing another query

If another query returns a scalar number, you can reuse it.

Assume a query named **Declaring Variables** returns `10`:

```plaintext
let
    v1 = 10,      // integer (number)
    v2 = 3.14,    // decimal (number)
    sum = v1 + v2 + #"Declaring Variables",   // name has a space → wrap in #"..."
in
    sum    // 23.14
```

## M Language Data Types — Part 2 - **Text**

### What is `text` in M?

* A **scalar string** value (names, sentences, IDs).
    
* **Surrounded by double quotes**: `"Hello"`.  
    Even `"123"` is **text**, not a number.
    

### Declaring & concatenating

```plaintext
let
    name     = "Stacy",
    greeting = "Hello",
    msg      = greeting & " " & name     // "Hello Stacy"
in
    msg
```

* Use `&` to concatenate.
    
* Add spaces/punctuation as needed: `"Hello, " & name & "!"`
    

## Mixing text with numbers

You can’t concat a number directly—**convert it** first.

`Text.From(value)` – generic, culture-aware for many types

```plaintext
let
    qty   = 5,                      // number
    line  = "Qty: " & Text.From(qty)
in
    line                             // "Qty: 5"
```

### **Text.From()**

* `Text.From(value, [culture])` = Swiss-army knife. Converts *many* types (number, date, logical, etc.) to text with a basic/default rendering. Minimal control over formatting.
    

### **Number.ToText()**

* `Number.ToText(number, [format], [culture])` = Precision tool *just for numbers*. Lets you control **format strings** (decimals, thousands, percent, etc.) and culture.
    

| Aspect | `Text.From` | `Number.ToText` |
| --- | --- | --- |
| Input types | Many (number, date, datetime, logical, etc.) | Numbers only |
| Formatting control | Low (no format string) | High (supports format patterns) |

### Culture & formatting (when needed)

```plaintext
Number.ToText(1234.56, "N", "en-US")    // "1,234.56"
```

`"N"` is the **Number** format specifier used by `Number.ToText`.

**What it does:** formats the number with **thousands separators** and a **default number of decimal places** for the culture (typically **2**)

**Control decimals with a precision specifier**

* `"N0"` → `1,235`
    
* `"N2"` → `1,234.56`
    
* `"N4"` → `1,234.5600`
    

### Escaping quotes & special cases

2 double quotes either side ““ ““

```plaintext
let
    q1 = "He said ""Hi""",          // -> He said "Hi"
    // Name with spaces as a variable/step name:
    #"Customer Name" = "A. Lee",
    out = #"Customer Name"
in
    out
```

## Common `Text.*` helpers (80/20)

```plaintext
Text.Lower("ABC")            // "abc"
Text.Upper("abc")            // "ABC"
Text.Trim("  x ")            // "x"
Text.Clean("a b")            // remove non-printables
Text.Length("Hello")         // 5
Text.Contains("Power Query","query", Comparer.OrdinalIgnoreCase) // true
Text.Replace("a-b-c","-","/")           // "a/b/c"
Text.Split("a,b,c", ",")                 // {"a","b","c"}
Text.Combine({"A","B"},"; ")             // "A; B"
Text.Start("abcdef", 3)                  // "abc"
Text.End("abcdef", 2)                    // "ef"
```

### M Language Data Types — **Logical (Boolean)**

**What it is:** A scalar that can be only `true` or `false` (nullable: can also be `null`). Used in comparisons, filters, and `if … then … else`.

### Basics

```plaintext
let
    input1 = 5,
    input2 = 6,
    eq  = input1 = input2,      // false
    neq = input1 <> input2      // true
in
    neq
```

**Text comparison is case-sensitive**

```plaintext
"Hi" = "hi"    // false
```

## M Language — Null & Date/Time (Quick Study Note)

### Null **vs** Blank **vs** 0

* `null` = missing/unknown value (no type).
    
* **Blank/space** = a **text** value like `" "` (not null).
    
* `0` = a **number**.
    
* Math with `null` → `null`; text with `null` → **error** (coalesce first).
    

```plaintext
1 + null                 // null
"Hello" & null           // error
```

### Logical (Boolean) quickies

* Values: `true`, `false` (nullable: can be `null`).
    
* Comparisons: `= <> < > <= >=`
    
* Logic: `and or not`
    

```plaintext
5 <> 6 and "Hi" <> "hi"          // true (case-sensitive)
Text.Compare("Hi","hi", Comparer.OrdinalIgnoreCase)=0   // true
```

## M Language — Date/Time (Quick Study Note)

### Date/Time Literal Constructors

Use lower-case **hash** literals:

* **Date:** `#date(YYYY, MM, DD)`
    
* **Time:** `#time(HH, MM, SS)`
    
* **DateTime:** `#datetime(YYYY, MM, DD, HH, MM, SS)`
    
* (Also: `#datetimezone(...)`)
    

```plaintext
let
  d  = #date(2025, 5, 23),
  t  = #time(10, 15, 25),
  dt = #datetime(2025, 5, 23, 10, 15, 25)
in dt                                          // 5/23/2025 10:15:25 AM
```

### Combine a date and a time

Don’t use `&` (that makes **text**). Build a real datetime:

```plaintext
let
  d = #date(2025,5,23),
  t = #time(10,15,25),
  dt = #datetime(Date.Year(d), Date.Month(d), Date.Day(d),
                 Time.Hour(t), Time.Minute(t), Time.Second(t))
in dt         // 5/23/2025 10:15:25 AM
```

## Formatting & Parsing (culture-aware)

* To text:
    

```plaintext
Date.ToText(d, "dd MMM yyyy", "en-GB")          // "23 May 2025"
Time.ToText(t, "HH:mm:ss")
DateTime.ToText(dt, "yyyy-MM-dd HH:mm:ss")
```

* From text:
    

```plaintext
Date.FromText("23/05/2025", "en-GB")   // 5/23/2025
```

## M Language — Basic Operations - Arithmetic operation

### 1 ) Operators: `+ - * / ^ rem`

```plaintext
let
  x = 10, y = 5,
  Sum   = x + y,        // 15
  Diff  = x - y,        // 5
  Prod  = x * y,        // 50
  Div   = x / y,        // 2
  Pow   = Number.Power(x,2)  // 100   (x ^ 2)
  Mod   = Number.Mod(x, y)     // 1  (remainder) (x rem 3)  
in  [Sum=Sum, Diff=Diff, Prod=Prod, Div=Div, Pow=Pow, Mod=Mod]
```

**Tips**

* Division by 0 → error; guard first.
    
* If values might be text, convert: `Number.From(text)`.
    

---

### 2) M Language — Basic Operations - Comparison (returns logical)

Operators: `= <> < > <= >=`

```plaintext
5 = 5      // true
5 <> 6     // true
"Hi" = "hi" // false (M is case-sensitive)
```

Case-insensitive text compare:

```plaintext
Text.Compare("Hi","hi", Comparer.OrdinalIgnoreCase) = 0   // true
```

---

## 3) Logical (booleans)

Operators: `and or not` *(short-circuiting)*

```plaintext
true and false   // false
true or false    // true
not false        // true
```

With conditions:

```plaintext
let
  x = 4, y = 10,
  Both  = (x = 4) and (y = 11),   // false
  Either= (x = 4) or  (y = 100),  // true
  Invert= not (x = 4)             // false
in  [Both=Both, Either=Either, Invert=Invert]
```

**Readability:** use parentheses around each condition.

---

## 4) Null behavior (important)

* Math with `null` → `null`: `1 + null` = `null`
    
* Text with `null` → **error**: `"Hi" & null` → error  
    Guard/coalesce:
    

```plaintext
let 
v = 5         // Hi 5 
// v = null   // Hi
in 
"Hi " & (if v=null then "" else Text.From(v))
```

* Logical tests with `null` return `null`; test for null explicitly.
    

---

## 5) Operator precedence (highest → lowest)

1. `^`
    
2. `* / rem`
    
3. `+ -`
    
4. Comparisons (`= <> < > <= >=`)
    
5. `not`
    
6. `and`
    
7. `or`  
    Use parentheses to make intent clear.
    

---

## M Language — If / Else

### Syntax

```plaintext
if <condition> then <value-if-true> else <value-if-false>
```

* All keywords are **lowercase**.
    
* `<condition>` must evaluate to **true/false** (logical).
    
* The two result branches should be the **same type** (both text, both number, etc.).
    

### Simple example

```plaintext
let
  n1 = 10,
  n2 = 11,
  result = if n1 > n2 then "Greater" else "Smaller"
in
  result
```

## Text example (case-sensitive)

```plaintext
let
  q = "Q1",
  msg = if q = "Q1" then "This is Quarter 1" else "Unknown quarter"
in
  msg
```

## Case-insensitive compare

```plaintext
if Text.Compare(q, "q1", Comparer.OrdinalIgnoreCase) = 0
then "This is Quarter 1" else "Unknown"
```

## Nested if (readable pattern)

Use parentheses to keep it clear:

```plaintext
let
  q = "Q3",
  msg =
    if q = "Q1" then "Quarter 1" else
    (
      if q = "Q2" then "Quarter 2" else
      (
        if q = "Q3" then "Quarter 3" else "Quarter 4"
      )
    )
in
  msg
```

## “Else-if” style (cleaner)

Just chain `else if` (same as nested, easier to read):

```plaintext
let
    Quter = "Q3",
    result = if  Quter = "Q1" then "This is Quter 1 " else
             (if Quter = "Q2" then "This is Quter 2 " else
             if Quter = "Q3" then "This is Quter 3 " else "This is Quter 4 " ) 
in
    result   // This is Quter 3 
```

## With booleans and math

```plaintext
let
  x = 5, y = 3,
  verdict = if (x > y) and (x - y >= 2) then "OK" else "Check"
in
  verdict
```

## Null-safe condition

Comparisons with `null` return `null` (not false). Guard first:

```plaintext
if q <> null and q = "Q1" then "Quarter 1" else "Unknown"
```

**Cheat line:** keep results the same type, use `else if` for readability, wrap complex conditions in parentheses, and guard `null` before comparing.

## Power Query Parameters — Quick Study Note

### What is a Parameter?

A **named value** (number, text, date, logical, etc.) you define once and **reuse across queries** for filters, calculations, and connection settings. It removes hard-coding and makes refreshes flexible.

### Why use them?

* **Reusability:** one value → many queries.
    
* **Maintainability:** change in one place updates everywhere.
    
* **Flexibility:** swap servers, databases, or filter cutoffs.
    
* **Performance:** push filters early (e.g., SQL folding).
    

### How to create

**Power Query Editor → Home → Manage Parameters → New Parameter**

* Name, Description (optional)
    
* **Type**: Number / Text / Date / True/False
    
* **Suggested Values**: Any value, List of values, or Query
    
* Set **Current Value** (used at refresh)
    

### Typical uses

1. **Filter rows**
    

```plaintext
let
  CutoffDate = #"Cutoff Date",                    // date parameter
  Filtered = Table.SelectRows(Source, each [OrderDate] >= CutoffDate)
in
  Filtered
```

2. **Switch connections**
    

```plaintext
let
  Server = #"Server Name",                        // text parameter
  Db     = #"Database Name",
  Source = Sql.Database(Server, Db)
in
  Source
```

3. **Business rules**
    

```plaintext
let
  Score = #"Score Parameter",                     // number parameter
  Grade = if Score >= 90 then "A"
          else if Score >= 80 then "B"
          else if Score >= 70 then "C"
          else "D"
in
  Grade
```

## Power Query M — Built-in vs Custom Functions (

### Built-in functions

Predefined helpers like:

* `Number.IsEven(6)` → `true`
    
* `Number.IsOdd(7)` → `true`
    
* `Text.Upper("abc")`, `Date.Year(#date(2025,5,1))`, `Table.SelectRows(...)`
    

They each do one specific task. Names are **case-sensitive** (e.g., `Number.IsEven`, not `number.iseven`).

### Custom functions (your own)

**Shape:**

```plaintext
FunctionName = (param1 as number, param2 as text) => <expression>
```

* Parameters can be annotated: `as number`, `as text`, `as list`, `as date`, `as datetime`, `as logical`.
    
* The body (`<expression>`) can be a single expression **or** a full `let … in` block.
    

### 1) Example

```plaintext
let
    AddFunction = (num1 as number,num2 as number) => 
        num1 + num2
in
    AddFunction(5,10)  // 15
```

### 2) Return a label based on a number

```plaintext
sign_cf = (n as number) =>
    if n > 0 then "Positive"
    else if n = 0 then "Zero"
    else "Negative"
```

### 3) Function with its own `let … in` (clear & scalable)

```plaintext
let
    TotalProfit= (sellprice as number,buyprice as number , quntity as number ) =>
    let
        revinue = sellprice * quntity,
        cost = buyprice * quntity,
        Profit = revinue-cost
    in 
        Profit
in
    TotalProfit(20,10,50)
```

---

## Calling vs. Invoking

* **Direct call in code:** `revenue_cf(120, 2)` → `120`
    
* **Invoke via UI:** If you just reference the function name as the query output, Power Query shows an **Invoke** button to supply arguments interactively (creates a new query per invocation).
    

## Power Query M — Text Functions

### Test table

| Product ID | Product Name |
| --- | --- |
| 1 | ␠Apple iPhone 14 Pro␠ |
| 2 | SAMSUNG galaxy s22 |
| 3 | Sony Noise Cancelling Headphones |
| 4 | LG UltraWide Monitor |
| 5 | Apple Watch Series 7 |
| 6 | Fitbit Charge 5 |
| 7 | Razer Gaming Mouse |
| 8 | Google Pixel 6 |
| 9 | Bose QuietComfort 35 |
| 10 | canon camera␠␠ |

Legend: `␠` marks intentional spaces (leading/trailing) to test `Text.Trim`.

---

### Core functions (with commented results)

```plaintext
Text.Length("Hello World")                // 11  (spaces count)
Text.Upper("Hello")                       // "HELLO"
Text.Lower("Hello")                       // "hello"
Text.Trim("  Hello  ")                    // "Hello" (removes leading/trailing)
Text.Start("Hello World", 5)              // "Hello"
Text.End("Hello World  ", 5)              // "World"  (trim first if needed)
Text.Replace("23/05/2025", "/", "-")      // "23-05-2025"
Text.Contains("Power Query","query")      // false (case-sensitive)
Text.Contains("Power Query","query", Comparer.OrdinalIgnoreCase) // true
```

---

### In a table (Custom Column patterns)

### 1) Length of Product Name

```plaintext
Text.Length([Product Name])               // e.g., "Apple iPhone 14 Pro" → 20
```

### 2) Upper/Lower based on a condition

```plaintext
if [Product ID] = 1 or [Product ID] = 2
then Text.Lower([Product Name])           // rows 1–2: lowercased
else Text.Upper([Product Name])           // others: UPPERCASED
```

### 3) Trim then take first N chars

```plaintext
Text.Start( Text.Trim([Product Name]), 5) // row 1 "␠Apple..." → "Apple"
```

### 4) Classify by last character (after trim)

```plaintext
let last = Text.End(Text.Trim([Product Name]), 1)
in  if last = "5" then "5 series"         // e.g., "Fitbit Charge 5" → "5 series"
    else if last = "6" then "6 series"    // e.g., "Google Pixel 6"  → "6 series"
    else "Other series"                   // others
```

### 5) Replace multiple words

```plaintext
Text.Replace(
    Text.Replace([Product Name], "Mouse", "Computer"),
    "Monitor", "Computer"
)
// "Razer Gaming Mouse"  → "Razer Gaming Computer"
// "LG UltraWide Monitor"→ "LG UltraWide Computer"
```

### 6) Flag computer products (case-insensitive search)

```plaintext
if Text.Contains([Product Name], "Monitor", Comparer.OrdinalIgnoreCase)
   or Text.Contains([Product Name], "Mouse", Comparer.OrdinalIgnoreCase)
then "Computer products"                  // rows 4 & 7
else "Non-computer products"
```

---

## tips

* **Case-sensitive by default.** Use `Comparer.OrdinalIgnoreCase` when needed.
    
* **Spaces matter.** `Text.Length` counts them; `Text.Trim` before compare/slice.
    
* **Trailing spaces break matches.** Always trim before `Text.End/Start/=` checks.
    
* **Nulls throw on concat.**
    
    ```plaintext
    "Val: " & (if x=null then "" else Text.From(x))   // safe
    ```
    
* **Multi-line outputs:**
    
    ```plaintext
    Text.Combine({"A","B","C"}, "#(lf)")              // "A\nB\nC"
    ```
    

## Power Query M — Number Functions

### Test table

| EmployeeID | Name | Salary |
| --- | --- | --- |
| 101 | John Smith | 5000 |
| 102 | Emma Johnson | 7500 |
| 103 | Ava Williams | \-1200 |
| 104 | Lucas Brown | 3200 |
| 105 | Mia Davis | 0 |
| 106 | Noah Miller | \-2500 |
| 107 | Olivia Moore | 9800 |
| 108 | Liam Wilson | 6200 |
| 109 | Sophia Taylor | 4300 |
| 110 | James Clark | \-1500 |

---

### Core number functions (single-value examples)

```plaintext
Number.IsOdd(5)                  // true
Number.IsOdd(6)                  // false

Number.IsEven(6)                 // true
Number.IsEven(5)                 // false

Number.Mod(7, 2)                 // 1    (remainder of 7 ÷ 2)
Number.Mod(6, 2)                 // 0

Number.Abs(-1200)                // 1200
Number.Abs(2500)                 // 2500

Number.Sign(9800)                // 1    (positive)
Number.Sign(0)                   // 0
Number.Sign(-1500)               // -1

Number.FromText("123")           // 123  (number)
Number.ToText(1234.56)           // "1234.56" (text)

Number.ToText(1234.56, "N2", "en-US") // "1,234.56" (formatted)
```

---

### In the table (Custom Column patterns)

### 1) Odd/Even flags via built-ins

```plaintext
// Is salary odd?
Number.IsOdd([Salary])                 // e.g., 5000 → false

// Is salary even?
Number.IsEven([Salary])                // e.g., 6200 → true
```

### 2) Odd/Even/Zero via remainder

```plaintext
let
    r = Number.Mod([Salary], 2)
in
    if [Salary] = 0 then "Zero"        // 0 first, or it looks even
    else if r = 0 then "Even"
    else "Odd"
```

### 3) Absolute salary (remove sign)

```plaintext
Number.Abs([Salary])                   // -1200 → 1200
```

### 4) Sign label (− / 0 / +)

```plaintext
let s = Number.Sign([Salary])
in  if s = 0 then "Zero"
    else if s = -1 then "Negative"
    else "Positive"
```

### 5) Convert text → number before math

*(If a column is text but should be numeric)*

```plaintext
// Example: [SalaryText] = "6200"
Number.FromText([SalaryText])          // 6200 (number)
```

### 6) Convert number → text for text functions/concat

```plaintext
"Salary: " & Number.ToText([Salary])   // "Salary: 5000"
```

---