# Optimizing Allocative Efficiency in Revenue Cycle Management 
## Analysis of healthcare insurance denial economics using Excel

**Tools:** Excel (Sensitivity Analysis, Data Tables, XLOOKUP), Financial Modeling

---

## 1. Summary
The status quo regarding operational managment for many healthcare clinics is to pursue 100% of denied insurance claims. While this maximizes gross revenue, it often destroys net utility

I created a risk-adjusted financial model to identify the economic floor, locating the point where labor costs of an appeal exceeds the probability-weighted recovery amount

## 2.  Dashboard
[Model Dashboard](dashboard_preview.png)
*Above: The "Scenario Switcher" allows users to toggle between Best, Base, and Worst-case operational conditions.*

## 3. Methodology & Key Findings
I created a scenerio analysis to stress-test insurance claim economics against variable labor costs and success probabilities

### The "Worst Case" Trap
In adverse conditions (Low Win Rate + High Labor Time), the Net ROI of a claim collapses to $6.71. This indicates that manual pursuit of low-value claims is a misallocation of human capital.

### Breakpoint Analysis (Sensitivity Findings)
* **The $25 Claim Floor:** Claims valued at $25 were found to be mathematically destructive. Even with a 60% win rate under the base conditions barely under the profit margin. 
* **The $50 Claim Volatility :** Claims at $50 are highly elastic. A 15-minute delay in processing can turn the ROI negative.
* **The $100 Labor Inelasticity:** In complex denial scenarios requiring 45+ minutes of work, claims under $100 may not even cover the opportunity cost of senior staff.

## 4. Recommendation:
Based on the modeling, I proposed a new Triage Protocol to optimize Net Yield:

**Tier I (High Yield)** | Value ≥ $200 **OR** Win Rate > 60% | **Manual Intervention** |
**Tier II (Standard)** | Value $100 – $200 | **Automated Batching** |
**Tier III (Divestiture)** | Value < $100 **AND** Win Rate < 30% | **Summary Write-Off** |

## 5. Project Files
* **[Download the Excel Model](Lee_Denial_ROI_Model.xlsx)** - Includes Scenario Switcher and Sensitivity Tables.
* **[Read the Decision Memo](Decision_Memo_Oct2023.pdf)** - Full academic defense of the Triage Protocol.
