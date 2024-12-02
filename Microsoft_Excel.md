---
title: "Excel and VBA"
author: "Aman Jindal"
description: "Study Notes"
---

## Burning Questions (figure out solutions):

 How to move focus to the formula bar while editing a cell, using the keyboard?

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

## Excel Ribbon Terminology:

| **Level**          | **Example**                      |
|---------------------|----------------------------------|
| **Tab**            | **Home**, **Insert**, **View**   |
| **Group**          | **Font**, **Alignment**          |
| **Command**        | **Bold**, **Italic**, **Underline** |
| **Contextual Tab** | **Chart Tools**, **Table Design**|

## Shift & F1-F12 Shortcuts:

| **F1 to F12**         | **Shift + F1 to F12**                                     |
|------------------------|----------------------------------------------------------|
| **F1**: Opens **Help** | **Shift + F1**: Displays **What’s This?** descriptions   |
| **F2**: Edit cell      | **Shift + F2**: Add/Edit **Comment/Note**                |
| **F3**: Paste Name     | **Shift + F3**: Opens **Insert Function** dialog         |
| **F4**: Repeat action  | **Shift + F4**: Find next occurrence                     |
| **F5**: Opens **Go To**| **Shift + F5**: Opens **Find and Replace** (Find tab)    |
| **F6**: Cycle focus    | **Shift + F6**: Cycle focus (reverse)                    |
| **F7**: Opens **Spelling** dialog | **Shift + F7**: Opens **Thesaurus** (older versions) |
| **F8**: Extend selection mode | **Shift + F8**: Add non-adjacent selection         |
| **F9**: Calculate all  | **Shift + F9**: Calculate active worksheet               |
| **F10**: Activates Ribbon KeyTips | **Shift + F10**: Opens **Context Menu**       |
| **F11**: Creates new chart sheet | **Shift + F11**: Inserts new worksheet         |
| **F12**: Opens **Save As** dialog | **Shift + F12**: Saves the workbook           |


## Alt & F1-F12 Shortcuts:

| **F1 to F12**         | **Alt + F1 to F12**                                      |
|------------------------|----------------------------------------------------------|
| **F1**: Opens **Help** | **Alt + F1**: Opens the **Insert Chart** dialog box      |
| **F2**: Edit cell      | **Alt + F2**: Opens the **Save As** dialog box           |
| **F3**: Paste Name     | **Alt + F3**: Opens the **Name Manager**                 |
| **F4**: Repeat action  | **Alt + F4**: Closes the Excel window                   |
| **F5**: Opens **Go To**| **Alt + F5**: (No default action)                        |
| **F6**: Cycle focus    | **Alt + F6**: Switches between open windows             |
| **F7**: Opens **Spelling** dialog | **Alt + F7**: Displays the **Document Recovery Pane** |
| **F8**: Extend selection mode | **Alt + F8**: Opens the **Macro** dialog box      |
| **F9**: Calculate all  | **Alt + F9**: Displays the **Code** for active worksheet |
| **F10**: Activates Ribbon KeyTips | **Alt + F10**: Maximizes the Excel window     |
| **F11**: Creates new chart sheet | **Alt + F11**: Opens the VBA editor            |
| **F12**: Opens **Save As** dialog | **Alt + F12**: (No default action)            |

## Ctrl & F1-F12 Shortcuts:

| **F1 to F12**         | **Ctrl + F1 to F12**                                      |
|------------------------|----------------------------------------------------------|
| **F1**: Opens **Help** | **Ctrl + F1**: Toggles the display of the Ribbon          |
| **F2**: Edit cell      | **Ctrl + F2**: Opens the **Print Preview** page          |
| **F3**: Paste Name     | **Ctrl + F3**: Opens the **Name Manager** dialog box     |
| **F4**: Repeat action  | **Ctrl + F4**: Closes the active workbook                |
| **F5**: Opens **Go To**| **Ctrl + F5**: Restores the size of the workbook window  |
| **F6**: Cycle focus    | **Ctrl + F6**: Switches to the next workbook window      |
| **F7**: Opens **Spelling** dialog | **Ctrl + F7**: Opens the **Move Window** command |
| **F8**: Extend selection mode | **Ctrl + F8**: Opens the **Resize Window** command  |
| **F9**: Calculate all  | **Ctrl + F9**: Minimizes the workbook window             |
| **F10**: Activates Ribbon KeyTips | **Ctrl + F10**: Toggles maximize/restore size   |
| **F11**: Creates new chart sheet | **Ctrl + F11**: Inserts a new **macro sheet**   |
| **F12**: Opens **Save As** dialog | **Ctrl + F12**: Opens the **Open File** dialog  |

## Ctrl & Ctrl+Shift + 1-9 Shortcuts:

| **Ctrl + 1-9**                  | **Ctrl + Shift + 1-9**                                    |
|----------------------------------|----------------------------------------------------------|
| **Ctrl + 1**: Opens **Format Cells** dialog | **Ctrl + Shift + 1**: Applies **Number Format**             |
| **Ctrl + 2**: Toggles **Bold** text         | **Ctrl + Shift + 2**: Applies **Time Format**              |
| **Ctrl + 3**: Toggles **Italic** text       | **Ctrl + Shift + 3**: Applies **Date Format**              |
| **Ctrl + 4**: Toggles **Underline**         | **Ctrl + Shift + 4**: Applies **Currency Format**          |
| **Ctrl + 5**: Toggles **Strikethrough**     | **Ctrl + Shift + 5**: Applies **Percentage Format**        |
| **Ctrl + 6**: Show/hide objects             | **Ctrl + Shift + 6**: Applies **Scientific Format**        |
| **Ctrl + 7**: Show/hide Ribbon (older versions) | **Ctrl + Shift + 7**: Adds a **border outline**         |
| **Ctrl + 8**: Toggles Outline view          | **Ctrl + Shift + 8**: Selects the **current region**       |
| **Ctrl + 9**: Hides selected rows           | **Ctrl + Shift + 9**: Unhides hidden rows                 |
| **Ctrl + 0**: Hides selected columns           | **Ctrl + Shift + 9**: Unhides hidden columns                 |


## Ctrl & Ctrl+Shift + A-Z and Special Characters Shortcuts:

| **Ctrl + A-Z / Special Characters**  | **Ctrl + Shift + A-Z / Special Characters**                |
|---------------------------------------|------------------------------------------------------------|
| **Ctrl + A**: Select all              | **Ctrl + Shift + A**: Inserts argument names into a formula|
| **Ctrl + B**: Toggles bold            | **Ctrl + Shift + B**: (No default action)                  |
| **Ctrl + C**: Copy                    | **Ctrl + Shift + C**: (No default action)                  |
| **Ctrl + D**: Fill down               | **Ctrl + Shift + D**: (No default action)                  |
| **Ctrl + E**: Flash Fill              | **Ctrl + Shift + E**: (No default action)                  |
| **Ctrl + F**: Opens Find and Replace  | **Ctrl + Shift + F**: Opens the Format Cells Font tab      |
| **Ctrl + G**: Opens Go To dialog      | **Ctrl + Shift + G**: (No default action)                  |
| **Ctrl + H**: Opens Replace dialog    | **Ctrl + Shift + H**: (No default action)                  |
| **Ctrl + I**: Toggles italic          | **Ctrl + Shift + I**: (No default action)                  |
| **Ctrl + K**: Inserts hyperlink       | **Ctrl + Shift + K**: (No default action)                  |
| **Ctrl + L**: Creates a table         | **Ctrl + Shift + L**: Toggles filters                      |
| **Ctrl + N**: Creates new workbook    | **Ctrl + Shift + N**: (No default action)                  |
| **Ctrl + O**: Opens workbook          | **Ctrl + Shift + O**: Selects cells with comments          |
| **Ctrl + P**: Opens Print dialog      | **Ctrl + Shift + P**: Opens Format Cells Font tab          |
| **Ctrl + R**: Fill right              | **Ctrl + Shift + R**: (No default action)                  |
| **Ctrl + S**: Saves workbook          | **Ctrl + Shift + S**: (No default action)                  |
| **Ctrl + T**: Creates a table         | **Ctrl + Shift + T**: (No default action)                  |
| **Ctrl + U**: Toggles underline       | **Ctrl + Shift + U**: Expands/collapses formula bar        |
| **Ctrl + V**: Paste                   | **Ctrl + Shift + V**: Opens Paste Special dialog           |
| **Ctrl + W**: Closes workbook         | **Ctrl + Shift + W**: (No default action)                  |
| **Ctrl + X**: Cut                     | **Ctrl + Shift + X**: (No default action)                  |
| **Ctrl + Y**: Redo                    | **Ctrl + Shift + Y**: (No default action)                  |
| **Ctrl + Z**: Undo                    | **Ctrl + Shift + Z**: (No default action)                  |
| **Ctrl + ;**: Inserts current date    | **Ctrl + Shift + ;**: Inserts current time                 |
| **Ctrl + `**: Toggles formula view    | **Ctrl + Shift + `**: (No default action)                  |
| **Ctrl + [**: Selects direct precedents | **Ctrl + Shift + [**: (No default action)                 |
| **Ctrl + ]**: Selects direct dependents | **Ctrl + Shift + ]**: (No default action)                 |
| **Ctrl + Enter**: Fills selection with entry | **Ctrl + Shift + Enter**: Enters array formula          |

## Alt & Alt+Shift + A-Z and Special Characters Shortcuts:

| **Alt + A-Z / Special Characters**       | **Alt + Shift + A-Z / Special Characters**                  |
|-------------------------------------------|-------------------------------------------------------------|
| **Alt + A**: Opens Data tab               | **Alt + Shift + A**: Group rows/columns in a range          |
| **Alt + B**: Opens the Power Query tab    |                                                            |
| **Alt + C**: Opens the Review tab         |                                                            |
| **Alt + D**: Opens Data menu (older versions) | **Alt + Shift + D**: Inserts the current date               |
| **Alt + F**: Opens File menu              | **Alt + Shift + F**: Opens Format Cells Font tab            |
| **Alt + G**: Opens Design tab (Chart tools) |                                                            |
| **Alt + H**: Opens Home tab               |                                                            |
| **Alt + J**: Opens PivotTable Analyze tab |                                                            |
| **Alt + K**: Opens Developer tab          |                                                            |
| **Alt + L**: Opens the Formulas tab       |                                                            |
| **Alt + M**: Opens the Formulas tab       |                                                            |
| **Alt + N**: Opens the Insert tab         |                                                            |
| **Alt + P**: Opens Page Layout tab        |                                                            |
| **Alt + Q**: Opens the "Tell me what you want to do" box |                                                         |
| **Alt + R**: Opens Review tab             |                                                            |
| **Alt + S**: Opens View tab               |                                                            |
| **Alt + T**: Opens Tools menu (older versions) | **Alt + Shift + T**: Inserts current time                   |
| **Alt + V**: Opens View tab               |                                                            |
| **Alt + W**: Opens View tab               |                                                            |
| **Alt + Y**: Opens Help tab               |                                                            |
| **Alt + Enter**: Starts a new line in a cell |                                                        |

## Chart Types and Data:

| **Type of Data**                          | **Recommended Chart Type**                                      | **Purpose**                                                   |
|-------------------------------------------|------------------------------------------------------------------|---------------------------------------------------------------|
| **Trends over Time**                      | Line Chart or Area Chart                                        | Shows changes or trends over a continuous time period         |
| **Comparing Categories**                  | Column Chart or Bar Chart                                       | Compares quantities across discrete categories                |
| **Proportions or Percentages**            | Pie Chart or Donut Chart                                        | Highlights the share of parts in a whole                      |
| **Relationships between Variables**       | Scatter Plot or Bubble Chart                                    | Displays correlations or relationships between two or more variables |
| **Hierarchical Data**                     | Treemap or Sunburst Chart                                       | Visualizes parts of a whole in a hierarchy                   |
| **Data Distribution**                     | Histogram or Box and Whisker Chart                              | Shows how data is distributed over intervals                 |
| **Ranking**                               | Bar Chart or Column Chart                                       | Compares items ranked by size or magnitude                   |
| **Geographic Data**                       | Map Chart                                                       | Displays data distribution across geographic locations        |
| **Progress Towards a Goal**               | Gauge Chart (not native, custom) or Bar Chart                  | Tracks progress toward a target                               |
| **Composition Over Time**                 | Stacked Area Chart or Stacked Bar Chart                         | Shows changes in composition across time                     |
| **Comparison of Parts to Whole**          | Stacked Column Chart or 100% Stacked Column Chart              | Highlights proportions in each category                      |
| **Large Dataset with Many Variables**     | Scatter Plot, Bubble Chart, or Heat Map                        | Provides insights into multidimensional data                 |
| **Project Timelines**                     | Gantt Chart (requires customization)                           | Tracks timelines and dependencies in projects                |
| **Flow or Process Data**                  | Sankey Diagram (requires custom add-ins)                       | Illustrates flow between processes                           |
| **Data with Negative and Positive Values**| Waterfall Chart                                                | Shows cumulative effect of values, such as profits/losses    |
| **Financial Data**                        | Candlestick Chart                                              | Tracks price movements, such as stock prices                 |

# Charts Format Pane Navigation:

| **Action**                 | **Shortcut**            |
|----------------------------|-------------------------|
| Open Format Pane           | **Ctrl + 1**           |
| Cycle focus to Format Pane | **F6** or **Shift + F6**|
| Navigate within the pane    | **Tab / Shift + Tab**  |
| Expand/collapse options    | **Enter**              |
| Adjust numeric values       | **Arrow Keys**         |
| Close the Format Pane       | **Esc**                |

# Chart Navigation:

| **Action**                                                                                   | **Shortcut**     |
|----------------------------------------------------------------------------------------------|------------------|
| Move between different element of a chart                                                    | **Alt + Arrow**  |
| Move inside a single element of a chart (like selecting individual data bars of a bar chart) | **Ctrl + Arrow** |

# Chart Tricks:

- **Dynamic Titles:** Just select the title box (don't press Enter/F2 etc) => Press `=`, and then the cell with arrow keys/mouse wherever your title is stored. This will help you in creating dynamic titles for your charts.
- **Creating Charts**
  - Select the data, and then the chart. Use recommended charts option (within Insert). Then go to All Charts. Over there, it is easy to get a preview, and see the list of all possible charts.
  - Create a blank chart of whichever type you wish, and then select the data, separated by commas (Shift+F10 => Select Data). This is helpful if you are data is all over the place.
- **Keeping only certain entries in the Legend:** Click/Select the particular data series legend (yes you can do this! - selecting individual legend items), and then just press delete.

## Combination Charts:



## Custom Formatting Symbols:

| **Symbol**   | **Meaning**                                                                                      |
|--------------|--------------------------------------------------------------------------------------------------|
| `0`          | Displays a number, including leading or trailing zeros.                                          |
| `#`          | Displays a number but does not show extra zeros (e.g., does not pad with leading or trailing).   |
| `,`          | Divides the number by 1,000 for each comma.                                                      |
| `.`          | Decimal point.                                                                                   |
| `%`          | Multiplies the number by 100 and displays it as a percentage.                                    |
| `$`          | Adds a dollar sign (or other currency symbol, depending on regional settings).                   |
| `\`          | Escapes the next character, displaying it as literal text.                                       |
| `"Text"`     | Encloses literal text to display alongside numbers.                                              |
| `@`          | Represents text in the cell (used for custom text formatting).                                   |
| `;`          | Separates formatting for positive, negative, zero, and text values.                             |
| `[Color]`    | Specifies a color for the value (e.g., `[Red]`, `[Green]`, `[Blue]`).                            |
| `[Condition]`| Applies formatting based on conditions (e.g., `[>100]`).                                         |

## Custom Formatting Order:

| **Section**      | **Purpose**                                   | **Example**          |
|-------------------|-----------------------------------------------|----------------------|
| 1st Section       | Format for **positive values**               | `[Blue]#,##0`        |
| 2nd Section       | Format for **negative values**               | `[Red](#,##0)`       |
| 3rd Section       | Format for **zeros**                         | `[Green]Zero`        |
| 4th Section       | Format for **text**                          | `"Text: "@`          |

## Custom Formatting Examples:

| **Custom Format**                     | **Description**                                                     | **Example Input**    | **Displayed Output**      |
|---------------------------------------|---------------------------------------------------------------------|----------------------|---------------------------|
| `[Blue]#,##0;[Red](#,##0);[Green]0;Text: "@"` | Positive in blue, negative in red (in parentheses), zero in green, text prefixed with "Text:". | `123, -123, 0, Hello` | `123`, `(123)`, `Zero`, `Text: Hello` |
| `#,##0;[Red](#,##0);[Gray]Zero;;`     | Positive as-is, negative in red, zero in gray, **text hidden**.     | `123, -123, 0, World`| `123`, `(123)`, `Zero`, (hidden) |
| `[Blue]$#,##0.00;[Red]-$#,##0.00;[Green]"Zero Dollars";"Text: "@` | Positive as blue currency, negative as red currency, zero as "Zero Dollars", text prefixed with "Text:". | `123.45, -123.45, 0, Hi` | `$123.45`, `-$123.45`, `Zero Dollars`, `Text: Hi` |
| `0.00%;-0.00%;Zero Percentage;Text`   | Positive as percentage, negative as percentage with `-`, zero as "Zero Percentage", text as-is. | `0.123, -0.123, 0, Text`| `12.30%`, `-12.30%`, `Zero Percentage`, `Text` |
| `[Green]"Profit: "0;[Red]"Loss: "0;0;"Data: "@` | Adds "Profit" or "Loss" to numbers, "Data" to text, zero as-is.    | `200, -200, 0, Hello`| `Profit: 200`, `Loss: 200`, `0`, `Data: Hello` |
| `#,##0;[Red](#,##0);[Blue]"Zero Value";` | Positive and negative formatted, zero in blue, **text hidden**.    | `123, -123, 0, Hi`   | `123`, `(123)`, `Zero Value`, (hidden) |


## Custom Formatting More Examples:

| **Custom Format**           | **Description**                                                             | **Example Input** | **Displayed Output** |
|------------------------------|-----------------------------------------------------------------------------|-------------------|-----------------------|
| `0`                         | Displays numbers as is, including leading/trailing zeros if needed.         | `5`               | `5`                  |
| `0000`                      | Pads numbers with leading zeros to make 4 digits.                           | `5`               | `0005`               |
| `#,##0`                     | Displays numbers with thousand separators.                                  | `1234567`         | `1,234,567`          |
| `#,##0.00`                  | Displays numbers with two decimal places and thousand separators.           | `1234.5`          | `1,234.50`           |
| `$#,##0`                    | Adds a dollar sign and thousand separators.                                 | `1234567`         | `$1,234,567`         |
| `€#,##0.00`                 | Adds a Euro sign with two decimal places.                                   | `1234567.89`      | `€1,234,567.89`      |
| `¥#,##0`                    | Adds a Yen sign with thousand separators.                                   | `1234567`         | `¥1,234,567`         |
| `£#,##0`                    | Adds a Pound Sterling symbol with thousand separators.                      | `1234567`         | `£1,234,567`         |
| `$0,,`                      | Divides the number by 1,000,000 and displays in millions with a dollar sign.| `123456789`       | `$123`               |
| `$0,\B`                     | Divides the number by 1,000 and adds a `B` after it.                        | `123456789`       | `$123456 B`          |
| `$0,,\M`                    | Divides the number by 1,000,000 and adds `M` for millions.                  | `123456789`       | `$123M`              |
| `0.0E+00`                   | Displays numbers in scientific notation.                                    | `12345`           | `1.2E+04`            |
| `0%`                        | Multiplies by 100 and adds a percent sign.                                  | `0.25`            | `25%`                |
| `[Red]0;[Green]0;[Blue]0`   | Displays positive numbers in red, negative in green, and zeros in blue.     | `123, -123, 0`    | `123 (red)`          |
| `0" kg"`                    | Adds the text `kg` after the number.                                        | `123`             | `123 kg`             |
| `#\K`                       | Divides numbers by 1,000 and appends `K`.                                   | `1234567`         | `1235K`              |
| `[>1000]0,, "M";0`          | Displays numbers above 1,000 as millions (`M`); others as-is.               | `1500000`         | `1.5 M`              |
| `[Blue]#,##0;[Red]#,##0;0`  | Displays positives in blue, negatives in red, and zeros as-is.              | `123, -123, 0`    | `123 (blue)`         |
| `#,##0.00 "USD"`            | Displays numbers with `USD` appended.                                       | `1234.5`          | `1,234.50 USD`       |


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
-  **Expand groupings in a Pivot Table:** **Expand All:** groupings: Alt+A+J, or Alt+JT+X. **Expand Individually:** press Shift+F10 (Right click), and then E (Expand/Collapse), and choose whichever option you want
-  **Collapse groupings in a Pivot Table:** **Collapse All:** Alt+A+L or Alt+JT+P. **Collapse Individually:** press Shift+F10 (Right click), and then E (Expand/Collapse), and choose whichever option you want

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

## Solver and Goal Seek:

- For Goal Seek to work, there should be circular references. Remove the circular references.
- If you can't find the circular references, disable iterative calculations, and then they will show up marked by blue arrows.

##  Pivot Tables:

- They are composed of four building blocks:
  - **Columns:** Here you can put any of your categories (Ex: Region, Geographies) in which you want to summarize the data
  - **Rows:** Similar to columns. Rows and Columns give you a 2-D breakdown of your data. You can add sub-fields too within rows and columns
  - **Values:** This is the column whose summary (Sum, Count, Average) you wish to see in the table (example: Sales, Orders)
  - **Filters:** This is at a macro level, above the Pivot table itself, to filter the entire data for one or more values of a column. For example: You want your table to show the sales figures of only Northeast region, broken down by Industry, and Years. Then, you can put a FILTER for region, and select Northeast. In COLUMN you can put Industries, in ROWS you can put Order Dates, and in VALUES you can select Sales.
  - **Calculated Fields:** You can add a calculated column, in your Pivot Table, based on the columns in your data. `Alt+JT+J+F`. For example, difference between two columns such as sales and commissions to yield, net sales. However, the summary statistic that will be presented in the main table for calculated fields will only be SUM, and not anything else. **Best advice, avoid them, and add a column in your underlying table for whatever you are trying to do.**

## Data Tables:
 
- **You can create Data Tables, via Alt+H+T.** It will apply some sort of formatting by default. If you wish, **remove the formatting via, Alt+JT+S+C.**
- Data Tables create a structured table, out of your data stored as a table. Then you can refer to these tables by their names, and column names elsewhere.
- Other benefits include, **automatic totals/average/count/etc.** in the last row via **Ctrl+Shift+T**. Filtering/sorting etc. is much easier.
- **Data Table Referencing:** Data_Table_Name[Column_Name]

## Data Table Relationships / Excel's Internal Data Model:

- **Overview:** If you have multiple Data Tables, then we can define relationships between them. By relationship, I mean that one table has one column that has unique values (such as name of states and the region to which each belongs), while the other table has a column that repeatedly uses the names of those states (such as a table containing record of sales in different states). Now, we don't need to ~~VLOOKUP~~/Index-Match, region from the Regions data-table to the Sales data-table. We can define the relationship between them using the State column in both the tables. **Such relationships only work if one of the data-table has unique values.**
- **How to do:** `Alt+A+DM+A`, then you can define the relationship.
- **Excel's Internal Data Model:** The relationships above get stored in Excel's Internal Data Model. We can excess the Internal Data Model via, `Alt+A+DM`. If we have a very large dataset running into millions of rows, then we can't get that into a spreadsheet. We need to load that directly into the Internal Data Model.

## Power Pivots:

- **Create Power Pivots via Alt+N+V+D** These are more powerful versions of Pivot Tables. We can build them using columns from different tables, provided the relationships between different tables have been defined as explained in the Data Table Relationships section above. 
- **Calculated Columns:** We can create customized new columns from other columns. We can also use them as rows or columns in the Power Pivots.
- **What are Measures in Power Pivots:** These are measures that summarize the data, such as sum, count. The difference in **Power Pivots** is that we can create our own customized measures (**Explicit Measures**). In standard **Pivot Tables**, we are restricted to the measures (**Implicit Measures**) provided by Excel.  To create an Explicit Measure (Power Pivot -> Measures)
- **Examples of Functions:** SUMX, AVERAGEX, MAXX, MINX, RANKX, COUNTX, CALCULATE(<Expression>, <Filter 1>, <Filter 2>, …), FILTER(<Table>, <Filter Expression>), ALL(<Table>), RELATED(<Column Name>)
- **KPIs (Key Performance Indicators):** We can define these in Power Pivots. Values can be checked against, the KPIs, to display visual indicators that if values have met the KPIs. You need **Explicit Measures** for KPIs. Implicit measures won't work. First, define Explicit Measures, and then use them via (Power Pivot -> KPIs)

## Database Functions:

- **DSUM:** DSUM(Database, Field, Criteria). 
  - **Database** is your Data Table (select everything including the headers). 
  - **Field** is the column that you want to operate upon. While entering it in the formula, we only need to enter the header (column name). If you select the entire column, it will result in a #Value error. 
  - **Criteria** is the combination of other column values for which you want the total of the field column (It is entered along with the column names). 
    - The Criteria column names should be entered in the same order as they appear in the Database. However, you can skip columns if they aren't required. 
    - Further, you can add the same column more than once, if you have multiple conditions based on that column. Only one condition can be entered in one column. 
    - For example, if the Date should be less than Aug 1, 2024 and greater than July 1, 2024, then you can add two columns for dates.  
    - You can have multiple rows of criteria. All the conditions in one row are joined by `AND`. Rows are joined by `OR`.
    - Do not include blank rows in criteria. Excel would interpret that as no criteria, and since rows are joined by `OR`, you will get the sum/etc. of the entire Field column.


