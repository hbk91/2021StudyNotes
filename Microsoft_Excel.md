---
title: "Excel, VBA, & Others"
author: "Aman Jindal"
description: "Study Notes"
---

## Formatting:

- **Display Share Prices and EPS:** upto two decimal places, because that's how they are displayed by convention
- **Share Count:** We also usually use at least 1 decimal place, sometimes up to 2-3, to display the company's share count. 
- **Valuation Multiples:** Usually 1 decimal place for valuation multiples
- **Percentages:** One decimal place as well - even if the financial figures in the model have 0 decimal places

## Excel Ribbon Dictionary:

- **File:** F
- **Home:** H
- **Insert:** N
- **Data:** A
- **Formulas:** M
- **View:** W
- **Page Layout:** P
- **Review:** R
- **FactSet:** S
- **S&P Capital IQ:** G

## Excel Keyboard Shortcuts:

- **Enter text/formula in the formula bar instead of the cell:** `F2`, and the `Ctrl+A`. Only, works if the cell is empty. If the cell has something, `Ctrl+A` would just select the cell contents. Try to find if this can be achieved somehow. It is a real pain, to click in the formula bar. 
- **Group rows/columns:** Alt+A+G+G
- **Ungroup rows/columns:** Alt+A+U+U
- **Collapse a grouped range:** To collapse an already grouped range of rows: Alt+A+H
- **Expand a already grouped and hidden range:** Alt+A+J
- **Hide Rows:** Ctrl+`9`, **Unhide Rows:** Ctrl+Shift+`9`
- **Hide Columns:** Ctrl+`0`, **Unhide Rows:** Ctrl+Shift+`0`
- **Zoom In** Ctrl+Alt+`+`, **Zoom Out:** Ctrl+Alt+`-`
- **Add row/column above/to the left of the selected row/column**: Ctrl+`+`, **Delete selected row/column:** Ctrl+`-`
- **Zoom to a particular %:** Alt+W+Q;
- **Page Break:** Alt+P+B+I
- **Insert Link** (Outlook, Excel, Word, PPT, etc): Ctrl+K
- **Open a new view of the same Excel File:** Alt+W+N
- **Highlight precedent cells:** Ctrl+`[`
- **Highlight dependent cells:** Ctrl+`]`
- **Trace Direct Precedents and Dependents:** Ctrl+`[` and Ctrl+`]` 
-  **Trace All (Direct+Indirect) Precedents and Dependents:** Ctrl+Shift+`[` and Ctrl+Shift+`]`
-  **Name Manager:** Ctrl+F3,  or Alt+M+N
-  **New Line while entering text in a cell:** Alt+Enter
-  

## FactSet Shortcuts:


## Capital IQ Shortcuts:


## PitchBook Shortcuts:


## Excel Logical Conditions: 

- **IF:** Returns true values for all conditions that evaluate to non-zero
- **OR Condition:** `+`  IF((Q:Q="Apple")+(S:S="Banana"),R:R,""), will give all rows in R, where Q has Apple or S has Banana 
- **AND Condition:** `*` IF((Q:Q="Apple")*(S:S="Banana"),R:R,""), will give all rows in R, where Q has Apple and S has Banana
- **NOT Condition:** `-` IF((Q:Q="Apple")-(S:S="Banana")=0,R:R,""), will give all rows in R, where Q has Apple and S doesn't has a Banana. If we don't put a zero in the condition, it would return values where S has a banana, and Q doesn't have an Apple, because the condition will become -1 in that case, and **IF returns a true for all non-zero values**. Such an issue doesn't arise in OR or AND, and hence we skipped it over there.

##  Excel Functions:

- **Missing Optional Arguments in Functions:** Suppose you have three optional arguments in a function, and you need to enter the last two and skip the first optional one. Then you need to enter the default value for the first optional argument (generally 1)
- **Indirect Function:** In this, we can enter a text, and the function will return the cells mentioned by that text
- **Match Function:** Gives the numeric position of an item in a range
- **Index Function:** Gives the content of the cell at the intersection of a row and a column. Usually the row and column number is figured out from the **Match** function
- **Using Indirect, and Match together:** `SUMIFS(INDIRECT("Quarters!$D$"&MATCH($B4,Quarters!$B$1:$B$51,0)&":$T$"&MATCH($B4,Quarters!$B$1:$B$51,0)),Quarters!$D$2:$T$2,"<="&E$2,Quarters!$D$2:$T$2,">"&D$2)`
- **Array Function:** It is a method to apply a function over a range of cells, instead of just one cell
- **Transpose:** This function works across multiple rows/columns. For example: Transpose(A1:E5)
- **Sortby:** Sort a column, table, row, based on any number of criteria. 
- **Index & Match:** `Index(Array, Row, Col) => Index(Entire Array, Match(Row Lookup Value, Row Array, 0), Match(Col Lookup Value, Col Array, 0))`
- **Xlookup:** General Format: `Xlookup(Lookup value, lookup array, return array)`, can easily return entire row/col array apart from lookup value. You can also lookup multiple values, just specify them as a range in the lookup value argument. **As a replacement for Index and Match =>** `Xlookup(Row lookup Value, Row Array, Xlookup(Col lookup value, Col Array, Entire Array))`
- **Xlookup Multiple Criteria Search:** `Xlookup(Lookup_Val_1&Lookup_Val_2, Lookup_Val_Array1&Lookup_Val_Array2, Return Array)`
- **IFS:** `IFS(logical_test1, value_if_true1, [logical_test2, value_if_true2], …)` It evaluates multiple conditions in a sequence and returns a value corresponding to the first condition that is TRUE. There is a workaround of adding a default value to `IFS`. Use the last logical condition as `TRUE`, and then add whatever default value you want. For example, `IFS(A1=2,Apple, A1=5, Banana, TRUE, Orange)`
- **COUNT:** All non-blank cells **with numbers**
- **COUNTA:** All non-blank cells
- **EDATE:** Extends a date by the number of months specified. `EDATE(Start Date, #Months)`. Months can be negative as well.
- **EOMONTH:** Outputs the last date of the month a date is extended to. `EOMONTH(Start Date, #Months)`. Months can be negative as well.
- **DATE:** `DATE(YEAR, MONTH, DATE)`

## List of Volatile Functions in Excel to avoid:

- Volatile functions are those that recompute everytime something changes in the excel file
- **VLOOKUP**
- **VLOOKUP multiple columns:** `VLOOKUP(B4,$B$2:$E$17,{2,3,4},FALSE)`. Alternatively, just use **XLOOKUP** as `XLOOKUP(B6,B3:B17,C3:E17)` . For backward compatibility, with older Excels, we use the `@` symbol, such as, `VLOOKUP(B4,$B$2:$E$17,@{2,3,4},FALSE)`. However, this addition of `@` will only yield the `2` column, that is the first argument in the argument list within `{}` 
- **HLOOKUP**
- **OFFSET**. For offset to be really useful, it has to return the entire range of cells, because Offset has the capability. INDEX and MATCH combo gives the value of only one cell. Syntax: OFFSET(Reference, #rows to shift, #cols to shift, [height of the block required], [width of the block required]). Note: The arguments within [] are optional.
 
## Excel tricks, behaviors:

- Always use `INDEX` and `MATCH`, instead of `CHOOSE` to select scenarios. `CHOOSE` doesn't accept the scenarios as a range in cells, and each scenario needs to be specified individually.
- Anything in double quotes, Excel assumes it is hard-coded.
- **Reversing a column:** Suppose the column is in AM24:AM29. Use the following trick: `INDEX($AM$24:$AM$28,ROWS($AM24:$AM$28))`, and drag the formula to as many items as in the original column.
- **Reversing a row:** Suppose the column is in AN39:AS39. Use the following trick: `INDEX($AN$39:$AR$39,1,COLUMNS(AN$39:$AR$39))`, and drag the formula to as many items as in the original row.
- **Creating a Date/Finding a year out of dates in a column:** `DATE(YEAR(MIN(Order_Table[Order Date])),1,1)`
- **Converting Text to Numbers:** **Enter 1 in a separate cell.** Then **Paste as special**, in all the columns where you wish to change text to numbers. While Pasting Special **choose the option Multiply**. The same can also be achieved by adding 0. Excel does't have a dedicated option in the ribbon for this. However, we can trick excel into doing this, via this trick. **Alternatively, do a Value(A1), in a separate cell, then paste as values in cell A1.**

## New Dynamic Array Functions introduced by Microsoft:

- You can reference the unknown ending point of ranges using the `#` symbol. For example: `N3:#`, if you don't know where the ending point is in column `N`
- However, results of dynamic functions create issues with conditional formatting, charts, and graphs.  
- **FILTER:** Example: FILTER(A1:B3, (B1:B3 > 85) * (A1:A3 <> "Bob"), "No Results"). Use logical operators (**+ for OR, * for AND**) to combine multiple conditions.
- SORTBY
- SORT
- XLOOKUP
- XMATCH
- UNIQUE
- SEQUENCE
- RANDARRAY

## Circular References:

- They mostly crop up while calculating interest expense/income, and cash balances together. 
- Also while calculating implied share price, when the #shares and implied share price are dependent on each other.
- Create a switch to handle circular references

## Data Tables:

- They are very helpful in data analysis, but not so much in pure financial modelling.

## Excel Error Types:

  1. **Most Common Errors:**

      - **#DIV/0!** Divide by zero error
      - **#REF!** Non-valid cell or range reference
      - **#NAME?** Function not recognized by Excel
      - **#VALUE!** Wrong type of input to function
      - **#NUM!** Non-valid number in calculation formula
      - **#N/A** Cannot find match for value with lookup function; if reference range are not of the same size in array functions
<br>

  2. **Not so Common:**

      - **#NULL!** Incorrect usage of Space in formulas, such as putting a space instead of a comma, colon in a formula. (Space is an intersection operator in excel, that gives the cells at the intersection of two ranges. Space as an operator is rarely used)

## Sensitivity Tables:

- Input and Output variables must be on the same spreadsheet
- **Alt+A+W+T**. This option is under Data and then What if analysis. This option is called Data Table (but actually these are sensitivity tables). Mind the difference from the Data Table described below.

## Data Tables:
 
- **You can create Data Tables, via Alt+H+T.** It will apply some sort of formatting by default. If you wish, **remove the formatting via, Alt+JT+S+C.**
- Data Tables create a structured table, out of your data stored as a table. Then you can refer to these tables by their names, and column names elsewhere.
- Other benefits include, **automatic totals/average/count/etc.** in the last row via **Ctrl+Shift+T**. Filtering/sorting etc. is much easier.
- **Data Table Referencing:** Data_Table_Name[Column_Name]

## Solver and Goal Seek:

- For Goal Seek to work, there should be circular references. Remove the circular references. I
- If you can't find the circular references, disable iterative calculations, and then they will show up marked by blue arrows.

## Database Functions:

- **DSUM:** DSUM(Database, Field, Criteria). 
  - **Database** is your Data Table (select everything including the headers). 
  - **Field** is the column that you want to operate upon. While entering it in the formula, we only need to enter the header (column name). If you select the entire column, it will result in a #Value error. 
  - **Criteria** is the combination of other column values for which you want the total of the field column (It is entered along with the column names). 
    - The Criteria column names should be entered in the same order as they appear in the Database. However, you can skip columns if they aren't required. 
    - Further, you can add the same column more than once, if you have multiple conditions based on that column. 
    - For example, if the Date should be less than Aug 1, 2024 and greater than July 1, 2024, then you can add two columns for dates.  

## Chrome Shortcuts:

- **Enable Keyboard Shortcuts:** Settings > See all settings > General tab > Scroll to Keyboard shortcuts and select Keyboard shortcuts on, save changes
- **Navigate Emails:** Use the `j` key to move down and `k` key to move up between emails.
- **Select Emails:** Press `x` to select an email. Repeat for multiple emails.
- **Delete Emails:** Once emails are selected, press `#` to delete them.
- **Focus on the search bar:** `/` (Forward Slash)

## VS Code Shortcuts:

- **Hide/Show Sidebar:** Ctrl+Alt+B
- **Focus on main Window:** Ctrl+1
- **Focus on Sidebar:** Ctrl+0
- **Stage & Commit:** Ctrl+Shift+G
- **Push to Git:** Open Command Pallete by Ctrl+Shift+P, then search `Push`
- **Open Keyboard Shortcuts Window:**  Ctrl+K Ctrl+S

## Windows Shortcuts:

- **Auto adjust the display width of all file Names in a Folder** Ctrl+`+` (Numeric Pad one). Regular one doesn't work. For Laptop => Find how to do it
