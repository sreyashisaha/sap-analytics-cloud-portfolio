# 📊 SAP Analytics Cloud — Sales Analytics Portfolio

> A end-to-end Sales Analytics story built in SAP Analytics Cloud (SAC), demonstrating core BI skills including KPI dashboards, time series analysis, cross tables with variance, combo charts, and AI-assisted exploration.

---

## 🔗 Live Tenant

| Field | Detail |
|---|---|
| **SAC Tenant** | [academy-t-sac.eu10.hcs.cloud.sap](https://academy-t-sac.eu10.hcs.cloud.sap) |
| **Data Source** | `Sales_Transactions_2020_2025` (SAC Samples) |
| **Time Range** | 2020 – 2025 |
| **Story Type** | Optimized Design Mode |
| **Theme** | SAP Morning Horizon |

---

## 📁 Story Structure

### Page 1 — Sales Overview
> High-level KPI snapshot and trend analysis

| Widget | Type | Measures / Dimensions |
|---|---|---|
| Total Net Sales | KPI Tile (Numeric Point) | NetValue |
| Total Quantity | KPI Tile (Numeric Point) | Quantity |
| Avg Order Value | KPI Tile (Numeric Point) | NetValue / Transactions |
| Total Transactions | KPI Tile (Numeric Point) | Count |
| Sales Trend | Time Series Line Chart | NetValue over SalesDate |
| Sales by Product Group | Bar Chart | NetValue × ProductGroup |

**Features used:** Reference Line, Threshold, Morning Horizon theme

---

### Page 2 — Sales Analysis
> Deep-dive cross-tabular and trend analysis with interactive filters

| Widget | Type | Measures / Dimensions |
|---|---|---|
| Sales by Product Group & Year | Cross Table | NetValue × ProductGroup × Year |
| Variance (Absolute & %) | Cross Table column | vs. Previous Year |
| Sales Trend by Product Group | Multi-line Chart | NetValue × SalesDate × ProductGroup |
| Sales by Distribution Channel | Bar Chart | NetValue × DistrChannel |
| Product Group Filter | Dimension Input Control | ProductGroup |
| Year Filter | Input Control | SalesDate (Year) |

**Features used:** Variance columns, Linked Analysis, Input Control

---

### Page 3 — Sales Order Analysis
> Order-level quantity and revenue analysis with combo chart

| Widget | Type | Measures / Dimensions |
|---|---|---|
| Sales Order by Product Group & Year  | Cross Table | Quantity × ProductGroup × Year  |
| Quantity Sold Over Time | Multi-line Chart | Quantity × SalesDate × ProductGroup |
| Revenue vs. Quantity | Combo Chart (Bar + Line) | NetValue (bars) + Quantity (line) × ProductGroup |
| AI Commenting / JustAsk | Smart Feature | Natural language data exploration |

**Features used:** Combo chart with secondary axis, Smart Insights / JustAsk

---

## 📐 Data Model

**Model:** `Sales_Transactions_2020_2025`
**Location:** My Files → Samples

| Field | Type | Description |
|---|---|---|
| `NetValue` | Measure | Revenue in EUR (millions) |
| `Quantity` | Measure | Units sold (thousands) |
| `ProductGroup` | Dimension | Electronics, Food, Furniture |
| `SalesDate` | Time Dimension | Daily, aggregated by Year/Month |
| `DistrChannel` | Dimension | Distribution channel |
| `Division` | Dimension | Business division |
| `CustomerName` | Dimension | Customer |
| `SalesOrg` | Dimension | Sales organisation |
| `CompanyCode` | Dimension | Legal entity |

---

## 📸 Screenshots

> Screenshots of each page are located in the `/screenshots` folder.

| File | Description |
|---|---|
| `page1-sales-overview.png` | KPI tiles + time series + bar chart |
| `page2-sales-analysis.png` | Cross table with variance + filters |
| `page3-sales-order-analysis.png` | Combo chart + quantity charts |

---

## 🚀 How to Explore This Story

1. Log in to the SAC tenant linked above
2. Navigate to **My Files → Samples**
3. Open the story: **Sales Analytics Portfolio**
4. Use the **input controls** on Page 2 to filter by Product Group, Year, or switch between NetValue and Quantity
5. Explore **Page 3** for order-level analysis and AI insights
---

## 👤 Author

**GE303485**
SAC Academy Student — SAP Analytics Cloud Fundamentals

---

## 📄 License

This project is for educational/portfolio purposes only.
Data source: SAP-provided sample data (`Sales_Transactions_2020_2025`).
