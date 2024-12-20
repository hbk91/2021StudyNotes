---
title: "Investment Banking General"
author: "Aman Jindal"
description: "Notes"
---

## Formatting Guidelines:

| **Element**                 | **Color**     | **Notes**                                                     |
|-----------------------------|---------------|-------------------------------------------------------------|
| **Hardcoded values**        | Blue          | Represents manually entered data.                           |
| **Input Boxes**             | Yellow        | Indicates cells where user inputs are required.             |
| **Values Pulled from other sheets** | Green | Shows data linked from other sheets or sources.             |
| **Calculations**            | Black         | Denotes formula-based data.                                 |
| **Text**                    | Mostly Black  | Black for standard text, adjusted for contrast on dark backgrounds (e.g., table headings). |

## Formatting:

- **Display Share Prices and EPS:** upto two decimal places, because that's how they are displayed by convention
- **Share Count:** We also usually use at least 1 decimal place, sometimes up to 2-3, to display the company's share count. 
- **Valuation Multiples:** Usually 1 decimal place for valuation multiples
- **Percentages:** One decimal place as well - even if the financial figures in the model have 0 decimal places

## Plotting a Dynamic Stock Price Line on a Football Field:

**Essentially we have to plot a scatter plot with stock price on one axis as all values, and on the other axis a large number for only one point, and zero for all the others. This is a standard trick to plot straight lines.**

- In your data for the football field, add a new row for the stock price. For one axis (doesn't matter x or y), add the stock price, for the other add a large number (like 1000/10,000) for the Min point and 0 for everything else.
- Next add the stock price data from above as a new cluster column/bar (depending upon how you are presenting the football field).
- Once plotted as a bar, go and manually edit the `SERIES` formula (excel automatically creates a series formula for each row/column plotted), to have x and y values:
  - **X-values**: The stock price range.
  - **Y-values**: 1000 and 0 values axis created above.
  - **SERIES Formula**: `SERIES(name, x_values, y_values, plot_order)`
    - `name`: Refers to the name of the data series. Can be a cell reference, range, or hard-coded text.
    - `x_values`: Specifies the range of data for the x-axis (categories or horizontal axis).
    - `y_values`: Specifies the range of data for the y-axis (values or vertical axis).
    - `plot_order`: Specifies the order in which the series appears in the chart (optional).
- Next, select the entire chart, and change the share price chart type to smooth scatter plot, and tick the scatter plot's axis as secondary axis.
- Now the x-axis labels are messed up. So in "Select data" for the entire chart fix the x-axis to your regular labels.
- Hide/Delete the secondary axis (Hide option is better, get in the habit of using it -> Format pane select axis labels as none).
- Format the share price line as you wish.

## Fixing the Dates Axis in a Stock Price/Volume Chart:

**Problem:** Have a fixed start date, end date and a small number of dates in between. While the data plotted is for the entire year.
**Solution:**