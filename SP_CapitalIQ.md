---
title: "S&P Capital IQ"
author: "Aman Jindal"
description: "Notes"
---

## **SNLTable Options**

| **Option**     | **Description**                                                | **Example**                                       |
|----------------|----------------------------------------------------------------|---------------------------------------------------|
| **MAG=**       | Sets magnitude (scales raw values into thousands, millions, billions). Works for dollar/amount fields, not ratios. | `{MAG=1000}` → show in thousands; `{MAG=1000000}` → show in millions |
| **CURRENCY=**  | Forces output in a specified reporting currency.               | `{CURRENCY=USD}` or `{CURRENCY=EUR}`              |
| **CCM=**       | Currency Conversion Method. Defines how FX rates are applied.  | `{CCM=MRSpot}` → most recent spot rate; `{CCM=Average}` → period average |
| **ORIENT=**    | Controls row/column layout of the returned table.              | `{ORIENT=FieldRows}` → fields in rows; `{ORIENT=FieldColumns}` → fields in columns |
| **MIStandard** | Applies S&P’s standard formatting style (used in MI Office templates). | `{MIStandard}`                                    |
| **SaveSetting**| Saves current orientation/formatting defaults for future queries. | `{SaveSetting}`                                   |
| **DateFormat=**| Controls how date labels appear.                               | `{DateFormat=YYYY-MM}`                            |
| **Missing=**   | Sets how missing data displays.                                | `{Missing=NA}` or `{Missing=0}`                   |
| **Decimal=**   | Specifies number of decimals shown in output.                  | `{Decimal=2}`                                     |

---

### Notes
- Multiple options can be combined inside one set of braces:  
  ```excel
  =SNLTable(..., "{MAG=1000000, CURRENCY=USD, ORIENT=FieldRows}")
