# Finance Dashboard — Power BI

A comprehensive financial analytics dashboard built for a fictional SaaS company ("Nexora Technologies"), covering expense tracking, budget vs actual analysis, profit margins, and financial forecasting.

## 📊 Dashboard Pages

### Page 1: Executive Summary
![Executive Summary](page1-executive-summary.png)

12 KPI cards (Total Actual Spend, Total Budget, Budget Variance %, Profit Margin %, Approval status breakdown), a monthly Budget vs Actual trend line, a department-wise spend comparison, and a category-wise spend breakdown.

### Page 2: Department & Category Analysis
![Department Analysis](page2-department-category.png)

A Department × Category matrix with conditional-formatting heatmap, a monthly spend trend by category, and an interactive department slicer.

### Page 3: Financial Forecast
![Forecast](page3-forecast.png)

A 6-month spend forecast using Power BI's built-in forecasting (exponential smoothing) with a 95% confidence interval.

## 🛠️ Tools & Techniques

- **Data generation:** Python (Pandas, NumPy) — generated a realistic, transaction-level synthetic dataset (~20,000 rows) with seasonality, YoY growth, and intentional data-quality issues for cleaning practice
- **Data cleaning:** Python/Pandas — handled duplicates, missing values, mixed date formats, inconsistent categorical values, and outliers (IQR method + domain judgment)
- **Data modeling:** Power BI — star schema (fact tables linked to Department, Category, and Calendar dimensions)
- **DAX:** 12+ measures including CALCULATE, DIVIDE, and time intelligence
- **Visualization:** Power BI — KPI cards, line charts, matrix heatmaps, donut charts, slicers, and built-in forecasting

## 📁 Files

- `Finance-Dashboard.pbix` — the Power BI file
- Screenshots of each dashboard page

## 🔑 Key Insights

- Software & Subscriptions is the highest-spend category (16.4% of total)
- Overall budget variance is +2.6% (mild overspend)
- Profit margin sits at 57.5%, driven mainly by the Enterprise SaaS segment
