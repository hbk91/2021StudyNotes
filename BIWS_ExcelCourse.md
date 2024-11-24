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
  
##  Excel Functions:

- **Missing Optional Arguments in Functions:** Suppose you have three optional arguments in a function, and you need to enter the last two and skip the first optional one. Then you need to enter the default value for the first optional argument (generally 1)
- **Indirect Function:** In this, we can enter a text, and the function will return the cells mentioned by that text
- **Match Function:** Gives the numeric position of an item in a range
- **Index Function:** Gives the content of the cell at the intersection of a row and a column. Usually the row and column number is figured out from the **Match** function
- **Using Indirect, and Match together:** `SUMIFS(INDIRECT("Quarters!$D$"&MATCH($B4,Quarters!$B$1:$B$51,0)&":$T$"&MATCH($B4,Quarters!$B$1:$B$51,0)),Quarters!$D$2:$T$2,"<="&E$2,Quarters!$D$2:$T$2,">"&D$2)`
- **Array Function:** It is a method to apply a function over a range of cells, instead of just one cell
- **Transpose:** This function works across multiple rows/columns. For example: Transpose(A1:E5)
- **Sortby:** Sort a column, table, row, based on any number of criteria. 

## List of Volatile Functions in Excel to avoid:

Volatile functions are those that recompute everytime something changes in the excel file

- VLOOKUP
- HLOOKUP
- OFFSET

## Some Simple Excel Tasks:

- **Reversing a column:** Suppose the column is in AM24:AM29. Use the following trick: INDEX($AM$24:$AM$28,ROWS($AM24:$AM$28)), and drag the formula to as many items as in the original column.
- **Reversing a row:** Suppose the column is in AN39:AS39. Use the following trick: INDEX($AN$39:$AR$39,1,COLUMNS(AN$39:$AR$39)), and drag the formula to as many items as in the original row.

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


