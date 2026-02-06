Session 20) DAX & Functions( Vlookup,Related,FirstNonBlank,IF,AND,IfError,Switch,Group by,Summeraze)
https://youtu.be/fRcSuM9QtFg?si=dzV2KsmFn5liDNqn

#  LookupValue:
- We can have lookupValue only on tables who doesn’t have relations, otherwise we have to use this formula:
  - # Related
  - Qtr Name = RELATED(Calendar_Table[Qtr Name])
- It has 3 parameters:
 (the result column name that we want show in our table)
    - We have to determined 2 common columns in 2 different table that are going to join.like :     - Date column in Calender table
    - And Date table in Sale Table
 
  <img width="887" height="232" alt="image" src="https://github.com/user-attachments/assets/40dd51d5-612f-4408-9ad2-ee8ce588b3c7" />
- Create a new Column (measure) >
- <img width="1477" height="326" alt="image" src="https://github.com/user-attachments/assets/84b19317-95af-4726-b937-797b82c845b3" />

# DAX LOOKUPVALUE – Detailed Explanation

## Formula
<img width="321" height="171" alt="image" src="https://github.com/user-attachments/assets/b5664793-3598-4c11-98ff-abcbd822ce91" />

- # What LOOKUPVALUE Does
- LOOKUPVALUE returns a value from one table by finding a matching value in another column.
- It is conceptually similar to Excel’s VLOOKUP, but works with columns and filter context.

<img width="404" height="414" alt="image" src="https://github.com/user-attachments/assets/21332f97-7250-4991-a0d2-dea206e3dd0e" />

- Breakdown of the Formula
- 1. Result Column
    - Calendar_Table[Qtr Name]
    -  Returns the quarter name (e.g. Q1 2024, Q2 2024).
- 2. Search Column
    - Calendar_Table[Date].[Date]
    - The column where the lookup happens.
    - .Date removes the time portion from a DateTime value.
- 3. Search Value
    - tblSales[Order Date].[Date]
    - The order date from the Sales table, also converted to Date only.
<img width="598" height="236" alt="image" src="https://github.com/user-attachments/assets/abe8deef-8814-48d4-bd80-16b4ce020ba0" />

# Example:
<img width="537" height="594" alt="image" src="https://github.com/user-attachments/assets/3b7e4cb3-0075-4230-8228-a0aa550ce281" />
# Important Notes
- Date Matching
  - Dates must match exactly
  - DateTime vs Date mismatch can return BLANK
  - Using .Date avoids this issue
    
- Single Match Requirement
    - LOOKUPVALUE must return exactly one row
    - Multiple matches → error
    - No match → BLANK

<img width="404" height="388" alt="image" src="https://github.com/user-attachments/assets/d61f5030-0dd4-4888-bebd-0ffac817ea2d" />
- Recommended Alternative (If Relationship Exists)
    - Qtr Name = RELATED(Calendar_Table[Qtr Name])

# Summary
  - Retrieves Quarter Name from Calendar table
  - Matches on Order Date
  - Useful when no relationship exists
  - Requires unique matching values

# FIRSTNONBLANK – DAX Function

## Purpose
`FIRSTNONBLANK` returns the **first non-blank value** in a column, evaluated within the **current filter context**, where a given expression is not BLANK.

---

## Syntax
<img width="260" height="174" alt="image" src="https://github.com/user-attachments/assets/323d8d84-5edf-41a1-bb79-d6552321d3b2" />
- Parameters
    - Column
        - The column from which the value is returned.
    - Expression
        - A DAX expression that is evaluated to determine whether the row is considered non-blank.

- How It Works
    - Iterates over the specified column in the current filter context
    - Evaluates the expression for each row
    - Returns the first value in the column where the expression is not BLANK
    - Stops evaluation after the first valid match

- Key Characteristics
    - Returns one value only
    - Does not guarantee sort order
    - Depends entirely on filter context
    - Commonly used with measures as the expression

- Typical Use Cases
    - Dynamic labels (Month, Quarter, Year)
    - Card visuals
    - Dynamic titles and tooltips

- Notes
    - If multiple values exist, the returned value depends on the model’s internal order
    - If no non-blank values are found, the result is BLANK
    - Not intended for numeric aggregation

- Alternative
<img width="718" height="61" alt="image" src="https://github.com/user-attachments/assets/fe22385d-6579-4c0c-b52f-f38e51e16281" />

# IF and AND – DAX Functions
---
## IF Function

### Purpose
`IF` evaluates a logical condition and returns **one value if the condition is TRUE** and **another value if it is FALSE**.

---

### Syntax
<img width="206" height="215" alt="image" src="https://github.com/user-attachments/assets/da67bf67-3db6-4463-91e7-50ab4fffacf2" />

- Parameters
    - Logical_Test
        - A condition that returns TRUE or FALSE.
    - Value_If_True
        - The value returned when the condition is TRUE.
    - Value_If_False
        - The value returned when the condition is FALSE.

# Example
- IF(tblSales[Revenue] > 1000, "High", "Low")


- Notes
  - Can return text, numbers, or BLANK
  - Frequently used in calculated columns and measures
  - Nested IFs are allowed but can reduce readability

# AND Function
- Purpose
  - AND checks whether all given conditions are TRUE.
- Syntax
<img width="223" height="182" alt="image" src="https://github.com/user-attachments/assets/41016443-1cd0-4841-a3f3-b1d87be3f610" />

# Example
<img width="315" height="175" alt="image" src="https://github.com/user-attachments/assets/333c5102-c7e3-400c-a3eb-fddefde74727" />

- Returns TRUE only if both conditions are TRUE.
- Logical Operator Alternative
- Instead of AND, you can use the logical operator && (recommended):
    - tblSales[Revenue] > 1000 && tblSales[Quantity] >= 10

<img width="570" height="330" alt="image" src="https://github.com/user-attachments/assets/dc53994f-ed31-4165-9cd0-f189bee28972" />

<img width="699" height="437" alt="image" src="https://github.com/user-attachments/assets/e5fce56f-3c46-415a-b3f7-68e01cde59d0" />

# IFERROR – DAX Function
---
## Purpose
`IFERROR` handles errors in DAX expressions by returning an **alternative value** when an error occurs.
It is commonly used to prevent visuals from showing errors such as division by zero.

---
## Syntax
<img width="183" height="168" alt="image" src="https://github.com/user-attachments/assets/763bae77-a525-43fa-bf1b-99263e4d13ee" />

- Parameters
    - Value
        - The DAX expression to evaluate.
    - Value_If_Error
        - The value returned if the expression results in an error.

- How It Works
    - Evaluates the given expression
    - If the expression returns a valid result → returns that result
    - If the expression throws an error → returns Value_If_Error

# Example
<img width="409" height="181" alt="image" src="https://github.com/user-attachments/assets/c647e614-4dfe-4d11-844f-b21102d678bd" />
- If Quantity is zero, the function returns 0 instead of an error.

- Common Use Cases
    - Prevent division-by-zero errors
    - Ensure clean visuals and measures
    - Replace errors with 0, "N/A", or BLANK()

- Notes
    - Catches errors only, not BLANK values
    - Overuse can hide data-quality issues
    - Should be applied intentionally

- Recommended Alternative
- For division operations, prefer DIVIDE():
<img width="235" height="217" alt="image" src="https://github.com/user-attachments/assets/16e78f49-d263-4395-8532-c3550113292b" />

- Summary
    - IFERROR replaces errors with a safe fallback value
    - Useful for error handling in DAX
    - DIVIDE() is safer and more explicit for arithmetic operations
 <img width="467" height="217" alt="image" src="https://github.com/user-attachments/assets/f6bda4d8-3c5a-4fda-9558-e6aff1ae5686" />
 
# Ex:  write a measure who extract the month name that  has maximum sale:
- create a new column in tblBudget ⇒ to bring Qtr name to budget table
  <img width="1158" height="579" alt="image" src="https://github.com/user-attachments/assets/a41bbb1d-489e-4b0b-bcb8-afda7c96dffd" />
- Now,create a new measure to find first QTR (month) that has max sale:
<img width="1607" height="435" alt="image" src="https://github.com/user-attachments/assets/700fee8d-bcda-4345-bed7-7552ddca3368" />












