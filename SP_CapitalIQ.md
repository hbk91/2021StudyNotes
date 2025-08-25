---
title: "S&P Capital IQ Pro"
author: "Aman Jindal"
description: "Notes"
---

# SNL & SPG Excel Functions Reference

This guide covers both the **legacy SNLxl functions** and their modern equivalents in **S&P Global MI Office (SPG)**.  
Syntax and behavior are nearly identical — just the prefix changes.

---

## 1. SNLData / SPGData
**Purpose:** Pull a single data point (cell) for one company/field/period.

**Syntax:**
= SNLData(dataset, SNL_ID, field_ID, key, tertiary_key, "{options}")  
= SPGData(dataset, Entity_ID, field_ID, key, tertiary_key, "{options}")

**Example:**
= SNLData("FF", 100162, "FF_ROE", "2024Q2", , "{CURRENCY=USD}")  
= SPGData("FF", 100162, "FF_ROE", "2024Q2", , "{CURRENCY=USD}")  
→ Returns JPMorgan’s **Return on Equity** for Q2 2024 in USD.

---

## 2. SNLTable / SPGTable
**Purpose:** Pull a full table (multiple IDs and fields at once).

**Syntax:**
= SNLTable(dataset, SNL_ID_range, field_ID_range, key_range, tertiary_key_range, "{options}")  
= SPGTable(dataset, Entity_ID_range, field_ID_range, key_range, tertiary_key_range, "{options}")

**Example:**
= SNLTable("FF", A2:A6, B2:B10, "MRQ", , "{MAG=1000, CURRENCY=USD}")  
= SPGTable("FF", A2:A6, B2:B10, "MRQ", , "{MAG=1000, CURRENCY=USD}")  
→ Returns most recent quarter’s financial fields in **thousands USD** for IDs in A2:A6.

---

## 3. SNLID / SPGID
**Purpose:** Look up an internal ID based on ticker, name, or identifier type.

**Syntax:**
= SNLID("IdentifierType", "Input")  
= SPGID("IdentifierType", "Input")

**Example:**
= SNLID("Ticker", "JPM")  
= SPGID("Ticker", "JPM")  
→ Returns JPMorgan Chase’s internal **Entity ID**.

---

## 4. SNLLabel / SPGLabel
**Purpose:** Returns the human-readable label for an ID or Field ID.

**Syntax:**
= SNLLabel(ID, [LabelType])  
= SPGLabel(ID, [LabelType])

**Example:**
= SNLLabel("FF_PTBV")  
= SPGLabel("FF_PTBV")  
→ Returns “**Price / Tangible Book Value**”.

---

## 5. SNLKey / SPGKey
**Purpose:** Generates a valid key (date/period) for use in data functions.

**Syntax:**
= SNLKey("KeyType", [Date])  
= SPGKey("KeyType", [Date])

**Examples:**
= SNLKey("Q", DATE(2024,12,31))   → "2024Q4"  
= SNLKey("MRQ")                   → "Most Recent Quarter"  
= SPGKey("LTM")                   → "Last Twelve Months"

---

## 6. SNLField / SPGField
**Purpose:** Returns the field code given a descriptive field name.

**Syntax:**
= SNLField("FieldName")  
= SPGField("FieldName")

**Example:**
= SNLField("Tangible Book Value Per Share")  
= SPGField("Tangible Book Value Per Share")  
→ Returns `"FF_TBVPS"`.

---

## 7. SNLUniverse / SPGUniverse
**Purpose:** Returns a dynamic list of IDs belonging to a defined universe or peer set.

**Syntax:**
= SNLUniverse("UniverseName")  
= SPGUniverse("UniverseName")

**Example:**
= SNLUniverse("US Banks > $10B Assets")  
= SPGUniverse("US Banks > $10B Assets")  
→ Returns IDs for all U.S. banks above $10B in assets.

---

## 8. SNLReport / SPGReport
**Purpose:** Pulls a pre-defined report into Excel.

**Syntax:**
= SNLReport("ReportName", "EntityID")  
= SPGReport("ReportName", "EntityID")

**Example:**
= SNLReport("Bank Profile", 100162)  
= SPGReport("Bank Profile", 100162)  
→ Returns the “Bank Profile” report for JPMorgan.

---

# Common Keys (SNLKey / SPGKey)

| **Code**   | **Meaning**                         | **Example Output** |
|------------|-------------------------------------|--------------------|
| MRQ        | Most Recent Quarter                 | "2024Q2"           |
| MRQ-1      | Prior Quarter                       | "2024Q1"           |
| MRQ-4      | Four Quarters Ago                   | "2023Q2"           |
| MRY        | Most Recent Year                    | "2023"             |
| MRY-1      | Prior Year                          | "2022"             |
| LTM        | Last Twelve Months                  | "LTM"              |
| YTD        | Year-To-Date                        | "YTD"              |
| FY2024     | Specific Fiscal Year                | "2024"             |
| 2024Q1     | Specific Quarter                    | "2024Q1"           |
| Date-based | Key from explicit Excel date input  | `SNLKey("Q", DATE(2024,12,31))` → "2024Q4" |

---

# Notes
- **dataset** codes: `"FF"` (Financials), `"MA"` (M&A), `"PR"` (Pricing), etc.  
- **key**: `"MRQ"`, `"LTM"`, `"FY2024"`, or generated dynamically with `SNLKey`/`SPGKey`.  
- **Options** (`{...}`) control:  
  - `MAG=` (magnitude: 1000, 1000000, etc.)  
  - `CURRENCY=` (reporting currency)  
  - `CCM=` (currency conversion method, e.g., MRSpot, Average)  
  - `ORIENT=` (FieldRows / FieldColumns)  
  - `Decimal=`, `Missing=`, `DateFormat=` etc.  
- SPG functions are the direct successors; syntax is the same, just the prefix changes.

===

# **SNLTable Options**

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


====