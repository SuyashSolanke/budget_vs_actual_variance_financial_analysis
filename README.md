# Corporate FP&A Financial Model & Analytics Dashboard (Google Sheets)

## Project Overview

Built an institutional-grade, multi-sheet Financial Planning & Analysis (FP&A) model and full-page interactive executive dashboard. The goal was to transmute disparate organizational transaction records into a dynamic reporting system that monitors variance control, identifies fixed vs. variable cost structures, tracks capital intensity, and projects rolling liquidity runways to support corporate strategic decision-making.

**Dataset:** Simulated Corporate Budgeting & Expense Data  
**Scope:** Multi-departmental fiscal tracking ($1.2B+ scale)

---

## Business Problem

The corporate finance team and senior leadership needed to solve critical business questions:
- How are business units tracking against allocated budgets in real time, and where is the operational leakage?
- What is the precise fixed baseline overhead required to keep the lights on versus activity-driven costs?
- What are the individual product lines and departmental revenue thresholds required to clear profitability safety margins?
- Is the organization generating sufficient operational cash flow to self-fund future expansion without equity dilution or high-interest debt exposure?

---

## KPI Summary

| KPI | Value | Metric Significance |
| :--- | ---: | :--- |
| **Annual Revenue Inflow** | $1.20B | High-velocity top-line generation |
| **Annual Budget Outflow** | $978.88M | Day-to-day capital utilization control |
| **Net Operational Cash Flow** | $223.14M | Total cumulative working capital reserve |
| **Average Quarterly Cash Burn** | $55.78M | Steady net liquidity added per quarter |
| **Target CAPEX Intensity** | 50.00% | Equal split between survival (OPEX) & growth (CAPEX) |

---

## Tools & Advanced Techniques Used

- **Google Sheets Architecture** (Separation of Raw Data Layer, Calculation Engines, and UI Layer)
- **Boolean Multi-Condition Arrays** (Simulating advanced logic via additive `=SUMIFS()`)
- **Matrix Lookups & Dynamic Drilldowns** (Interactive data validation drop-downs linked with `=VLOOKUP()`)
- **Linear Regression Forecasting** (Automated `=TREND()` / `=FORECAST()` baseline modeling)
- **Inline Micro-Visualizations** (Space-conscious trend mapping via `=SPARKLINE()`)
- **Custom UI System Design** (Gridline suppression, bespoke number formats, typographic hierarchies)

---

## Key Insights

- **Governance & Variance Control:** No business unit exceeded its $100\%$ allocated fiscal boundary. **R&D ($97.45\%$)** and **IT ($97.22\%$)** utilized their budgets most aggressively, meaning they run with a tight $<3\%$ emergency safety buffer. **HR ($93.63\%$)** maintains the highest capital cushion.
- **Predictive Expenditure Trends:** Running linear regression models across quarterly steps revealed a consistent downward spending trajectory moving into next fiscal year (**Q1 Forecast: $18.45M** dropping down to **Q4 Forecast: $17.39M**), indicating compounding operational optimization and leaner overhead.
- **Fixed vs. Variable Break-Even Scales:** High-revenue business units like **Logistics ($160.49M)** and **HR ($159.48M)** command exceptionally high fixed overhead baselines (Salaries, Facilities, Infrastructure), forcing them to cross an elevated break-even safety threshold (**$106.77M** and **$108.66M**) just to hit a $0 net profit mark.
- **Cash Fortress Stability:** The firm generates over **$53M to $58M in pure net cash flow every quarter**, building an ironclad cumulative liquidity runway of **$223.14M** by the end of Q4. The company is entirely self-funding and hyper-liquid.

---

## Strategic Recommendations

- **Address High-Utilization Sectors:** Allocate a nominal contingency budget expansion for R&D and IT in the next fiscal planning cycle, as their current $<3\%$ margin leaves them vulnerable to unexpected operational friction.
- **Protect Heavy Fixed Centers:** Closely monitor market volatility affecting Logistics. Because its break-even line is so high ($106.77M), even a slight dip in top-line revenue exposes the department to massive operating losses compared to structurally leaner units like Finance.
- **Capital Allocation Preservation:** Maintain the current **50% CAPEX Intensity Ratio**. The continuous, equal reinvestment into enterprise technology and long-term infrastructure ensures the firm outpaces market competitors without burning cash.

---

## Dashboard Features

- **Full-Page Unified Interface:** Completely designed on a gridline-free layer configured to fit an executive desktop monitor without scrolling.
- **Large-Scale KPI Block Cards:** Styled with bespoke string formatting codes (`$#,##0.00,,, "B"`) to scale large digits cleanly into billions.
- **Dynamic Departmental Selector Drilldown:** Allows viewers to click a drop-down filter and watch budget metrics and break-even sales values update across the entire sheet instantly.
- **Dual-Tone Inline Sparklines:** Embedded micro-charts mapped inside individual cells to visualize positive revenue momentum (green lines) versus asset expense streams (red lines).
- **Executive Chart Matrix:** Side-by-side synchronized data visualizations pulling variance blocks, cost boundaries, and liquidity growth lines onto a single dashboard workspace.

---

## Project Structure & Repository Architecture

```text
📦 Corporate-FP&A-Analytics-Dashboard
 ┣ 📂 screenshots
 ┃ ┣ 📜 Executive_Dashboard_Main.png
 ┃ ┣ 📜 Variance_Control_Matrix.png
 ┃ ┣ 📜 Expense_Forecast_Trends.png
 ┃ ┗ 📜 Cost_Behavior_Breakeven.png
 ┣ 📜 Financial_Model_Workspace.xlsx  <-- Compiled Production Spreadsheet Model
 ┣ 📜 Financial_Budgeting_Dataset.csv <-- Original Compressed Input Data Dump
 ┗ 📜 README.md                       <-- Portfolio Documentation (This File)
