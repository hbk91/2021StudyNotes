---
title: "BIWS Excel & VBA Course"
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

## List of Volatile Functions in Excel to avoid:

Volatile functions are those that recompute everytime something changes in the excel file

- **VLOOKUP**
- **VLOOKUP multiple columns:** `VLOOKUP(B4,$B$2:$E$17,{2,3,4},FALSE)`. Alternatively, just use **XLOOKUP** as `XLOOKUP(B6,B3:B17,C3:E17)` . For backward compatibility, with older Excels, we use the `@` symbol, such as, `VLOOKUP(B4,$B$2:$E$17,@{2,3,4},FALSE)`. However, this addition of `@` will only yield the `2` column, that is the first argument in the argument list within `{}` 
- **HLOOKUP**
- **OFFSET**. For offset to be really useful, it has to return the entire range of cells, because Offset has the capability. INDEX and MATCH combo gives the value of only one cell. Syntax: OFFSET(Reference, #rows to shift, #cols to shift, [height of the block required], [width of the block required]). Note: The arguments within [] are optional.

## Some Simple Excel Tasks:

- **Reversing a column:** Suppose the column is in AM24:AM29. Use the following trick: `INDEX($AM$24:$AM$28,ROWS($AM24:$AM$28))`, and drag the formula to as many items as in the original column.
- **Reversing a row:** Suppose the column is in AN39:AS39. Use the following trick: `INDEX($AN$39:$AR$39,1,COLUMNS(AN$39:$AR$39))`, and drag the formula to as many items as in the original row.
 
## Handy Tips & Tricks Excel:

- Always use `INDEX` and `MATCH`, instead of `CHOOSE` to select scenarios. `CHOOSE` doesn't accept the scenarios as a range in cells, and each scenario needs to be specified individually.

## New Dynamic Array Functions introduced by Microsoft:

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

## Excel Error Types:

  1. **Most Common Errors:**

      - **#DIV/0!** Divide by zero error
      - **#REF!** Non-valid cell or range reference
      - **#NAME?** Function not recognized by Excel
      - **#VALUE!** Wrong type of input to function
      - **#NUM!** Non-valid number in calculation formula
      - **#N/A** Cannot find match for value with lookup function; if reference range are not of the same size in array functions

  2. **Not so Common:**

      - **#NULL!** Incorrect usage of Space in formulas, such as putting a space instead of a comma, colon in a formula. (Space is an intersection operator in excel, that gives the cells at the intersection of two ranges. Space as an operator is rarely used)

## Sensitivity Tables:

- Input and Output variables must be on the same spreadsheet
  
## Solver and Goal Seek:

- For Goal Seek to work, there should be circular references. Remove the circular references. I
- If you can't find the circular references, disable iterative calculations, and then they will show up marked by blue arrows.

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
