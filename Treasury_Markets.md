---
title: "Treasury Markets"
author: "AJ"
description: "Notes"
---

## **Comparison of Treasury Securities Issuance in US and India**

| **Aspect**                | **United States**                                  | **India**                                      |
|---------------------------|----------------------------------------------------|------------------------------------------------|
| **Issuing Authority**     | U.S. Department of the Treasury                   | Reserve Bank of India (RBI) on behalf of GoI  |
| **Government Entity**     | U.S. Treasury                                     | Government of India (GoI)                      |
| **Types of Securities**   | - Treasury Bills (T-Bills) <br> - Treasury Notes <br> - Treasury Bonds <br> - Treasury Inflation-Protected Securities (TIPS) | - Treasury Bills (T-Bills) <br> - Government Bonds (G-Secs) <br> - Floating Rate Bonds (FRBs) <br> - Inflation-Indexed Bonds (IIBs) |
| **Maturity Periods**      | - T-Bills: ≤1 year <br> - T-Notes: 2 to 10 years <br> - T-Bonds: >10 years (typically 20-30 years) | - T-Bills: ≤1 year <br> - G-Secs: 5 to 40 years |
| **Auction Mechanism**     | Competitive and Non-Competitive Bidding via Federal Reserve | Conducted by RBI through E-Kuber (electronic platform) |
| **Market Participants**   | Banks, Mutual Funds, Pension Funds, Individuals, Foreign Investors | Banks, Mutual Funds, Insurance Companies, Foreign Portfolio Investors (FPIs), Individuals |
| **Retail Participation**  | TreasuryDirect (online platform for individuals)  | RBI Retail Direct (online portal for individuals) |
| **Foreign Investor Access** | Allowed under U.S. regulations, widely held globally | Limited but increasing; FPIs allowed with caps on investment |
| **Interest Payment**      | - Zero-coupon (for T-Bills) <br> - Fixed coupon (for Notes & Bonds) | - Zero-coupon (for T-Bills) <br> - Fixed & Floating (for G-Secs & FRBs) |
| **Liquidity**            | Highly liquid, actively traded worldwide          | Liquid but secondary market depth lower than the U.S. |
| **Risk Perception**      | Considered risk-free (backed by full faith and credit of the U.S. government) | Low risk but slightly higher than U.S. Treasuries due to sovereign credit profile |
| **Yield Determination**  | Market-driven through auctions and Federal Reserve influence | Market-driven but influenced by RBI’s monetary policy |


---

### **Day Count Conventions for Different Fixed-Income Securities in US Markets**

| **Security Type**    | **Day Count Convention** | **Reason for Convention** |
|---------------------|------------------------|--------------------------|
| **Treasury Bills (T-Bills)** | **Actual/360** | Used for discount instruments in the money market. |
| **Treasury Notes (T-Notes)** | **Actual/Actual** | Ensures accurate interest accrual, considering leap years. |
| **Treasury Bonds (T-Bonds)** | **Actual/Actual** | Standard for long-term U.S. government debt. |
| **Corporate Bonds** | **30/360** | Simplifies calculations for fixed-income investors and issuers. |
| **Municipal Bonds** | **30/360** | Standardized calculation method for state and local debt. |
| **Agency Debt (Fannie Mae, Freddie Mac, FHLB)** | **30/360** | Used for mortgage-backed and structured securities. |
| **Agency Debt (Ginnie Mae, some others)** | **Actual/360** | Aligns with Treasury market conventions for some government-backed debt. |

---

### **Example: T-Bill Discount Yield Calculation**
#### **Given Data:**
- **Face Value (\(F\))** = $1,000  
- **Purchase Price (\(P\))** = $980  
- **Days to Maturity (\(D\))** = 90  

Using the **discount yield formula**:

$$
y = \left( \frac{F - P}{F} \right) \times \left( \frac{360}{D} \right)
$$

Substituting the values:

$$
y = \left( \frac{1000 - 980}{1000} \right) \times \left( \frac{360}{90} \right)
$$

$$
y = \left( \frac{20}{1000} \right) \times 4 = (0.02) \times 4 = 8.00\%
$$

Thus, the **discount yield of this T-Bill is 8.00%**.

---