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

### Plotting a Dynamic Stock Price Line on a Football Field:

**Essentially we have to plot a scatter plot with stock price on one axis as all values, and on the other axis a large number for only one point, and zero for all the others. This is a standard trick to plot straight lines.**

    - In your data for the football field, add a new row for the stock price. For one axis (doesn't matter x or y), add the stock price, for the other add a large number (like 1000/10,000) for the Min point and 0 for everything else.
    - Next add the stock price data from above as a new cluster column/bar (depending upon how you are presenting the football field).
    - Once plotted as a bar, go and manually edit the `SERIES` formula (excel automatically creates a series formula for each row/column plotted), to have x and y values. X-values: the stock price range. Y-values: 1000 and 0 values axis created above.
      - **SERIES:** SERIES(name, x_values, y_values, plot_order). `name` Refers to the name of the data series. Can be a cell reference, range, or hard-coded text. `x_values:`Specifies the range of data for the x-axis (categories or horizontal axis). `y_values:` Specifies the range of data for the y-axis (values or vertical axis). `plot_order:` Specifies the order in which the series appears in the chart (optional).
    - Next select the entire chart, and change the share price chart type to smooth scatter plot, and tick the scatter plot's axis as secondary axis.
    - Now the x-axis labels are messed up. So in "Select data" for the entire chart fix the x-axis to your regular labels.
    - Hide/Delete the secondary axis (Hide option is better, get in the habit of using it -> Format pane select axis labels as none).
    - Format the share price line as you wish.
  