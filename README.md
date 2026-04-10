📊 SAP Analytics Cloud — Sales Analytics Portfolio

A end-to-end Sales Analytics story built in SAP Analytics Cloud (SAC), demonstrating core BI skills including KPI dashboards, time series analysis, cross tables with variance, combo charts, and AI-assisted exploration.

🔗 Live Tenant
FieldDetailSAC Tenantacademy-t-sac.eu10.hcs.cloud.sapData SourceSales_Transactions_2020_2025 (SAC Samples)Time Range2020 – 2025Story TypeOptimized Design ModeThemeSAP Morning Horizon

📁 Story Structure
Page 1 — Sales Overview

High-level KPI snapshot and trend analysis

WidgetTypeMeasures / DimensionsTotal Net SalesKPI Tile (Numeric Point)NetValueTotal QuantityKPI Tile (Numeric Point)QuantityAvg Order ValueKPI Tile (Numeric Point)NetValue / TransactionsTotal TransactionsKPI Tile (Numeric Point)CountSales TrendTime Series Line ChartNetValue over SalesDateSales by Product GroupBar ChartNetValue × ProductGroup
Features used: Reference Line, Threshold, Morning Horizon theme

Page 2 — Sales Analysis

Deep-dive cross-tabular and trend analysis with interactive filters

WidgetTypeMeasures / DimensionsSales by Product Group & YearCross TableNetValue, Quantity × ProductGroup × YearVariance (Absolute & %)Cross Table columnvs. Previous YearSales Trend by Product GroupMulti-line ChartNetValue × SalesDate × ProductGroupSales by Distribution ChannelBar ChartNetValue × DistrChannelProduct Group FilterDimension Input ControlProductGroupYear FilterInput ControlSalesDate (Year)
Features used: Variance columns, Linked Analysis, Input Control

Page 3 — Sales Order Analysis

Order-level quantity and revenue analysis with combo chart

WidgetTypeMeasures / DimensionsQuantity by Product GroupHorizontal Bar ChartQuantity × ProductGroupQuantity Sold Over TimeMulti-line ChartQuantity × SalesDate × ProductGroupRevenue vs. QuantityCombo Chart (Bar + Line)NetValue (bars) + Quantity (line) × ProductGroupAI Commenting / JustAskSmart FeatureNatural language data exploration
Features used: Combo chart with secondary axis, Smart Insights / JustAsk

📐 Data Model
Model: Sales_Transactions_2020_2025
Location: My Files → Samples
FieldTypeDescriptionNetValueMeasureRevenue in EUR (millions)QuantityMeasureUnits sold (thousands)ProductGroupDimensionElectronics, Food, FurnitureSalesDateTime DimensionDaily, aggregated by Year/MonthDistrChannelDimensionDistribution channelDivisionDimensionBusiness divisionCustomerNameDimensionCustomerSalesOrgDimensionSales organisationCompanyCodeDimensionLegal entity

📸 Screenshots

Screenshots of each page are located in the /screenshots folder.

File                                Description
page1-sales-overview.png            KPI tiles + time series + bar chart
page2-sales-analysis.png            Cross table with variance + filters
page3-sales-order-analysis.png      Combo chart + quantity charts


🚀 How to Explore This Story

Log in to the SAC tenant linked above
Navigate to My Files → Samples
Open the story: Sales Analytics Portfolio
Use the input controls on Page 2 to filter by Product Group, Year, or switch between NetValue and Quantity
Explore Page 3 for order-level analysis and AI insights

👤 Author
GE303485 SAC Academy Student — SAP Analytics Cloud Fundamentals

📄 License
This project is for educational/portfolio purposes only.
Data source: SAP-provided sample data (Sales_Transactions_2020_2025).
