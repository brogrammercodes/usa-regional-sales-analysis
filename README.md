# USA Regional Sales Analysis 📊

An end-to-end data analytics project on **Acme Co.'s 2014–2018 USA sales data** — from raw multi-sheet Excel data to a cleaned dataset, exploratory analysis, business insights, and an interactive Power BI dashboard.

---

## 🗂️ Project Summary

This project analyzes ~5 years of sales orders to identify the key revenue and profit drivers across **products, sales channels, and US regions**, uncover seasonal trends and outliers, and align performance against budgets. The findings feed a Power BI dashboard built to support strategic, data-driven decision-making.

The workflow covers:

- **Data Profiling & Cleaning** — verified schema across six source sheets, handled missing budgets, corrected data types, and standardized column names.
- **Data Wrangling & Merging** — joined sales orders with customers, products, regions, state-regions, and 2017 budgets into a single analytical table.
- **Feature Engineering** — derived total cost, profit, profit margin %, and order-level value.
- **Univariate & Bivariate Analysis** — distributions of revenue, margin, and unit price; product / channel / region breakdowns; customer segmentation.
- **Trend & Seasonality** — monthly and yearly sales patterns.
- **Outlier Detection** — extreme transactions at both ends of the revenue and unit-price spectra.
- **Correlation & Segmentation** — relationships between key metrics and customer clustering by revenue vs. profit margin.

---

## ❓ Problem Statement

Analyze Acme Co.'s 2014–2018 sales data to identify key revenue and profit drivers across products, channels, and regions; uncover seasonal trends and outliers; and align performance against budgets. Use these insights to optimize pricing, promotions, and market expansion for sustainable growth and reduced concentration risk.

## 🎯 Objectives

- Identify top-performing products, channels, and regions driving revenue and profit.
- Uncover seasonal trends and anomalies for optimized planning.
- Spot pricing and margin risks from outlier transactions.
- Inform pricing, promotion, and market-expansion strategies.

---

## 📁 Repository Contents

| File / Folder | Description |
|---|---|
| `EDA_Regional_Sales_Analysis.ipynb` | Main Jupyter notebook — full data cleaning, feature engineering, and 15 exploratory analyses with insights. |
| `Regional Sales Dataset.xlsx` | Raw source workbook (Sales Orders, Customers, Products, Regions, State Regions, 2017 Budgets). |
| `Sales_data(EDA Exported).csv` | Cleaned, merged, feature-engineered dataset exported from the notebook. |
| `SALES REPORT.pbix` | Interactive Power BI dashboard. |
| `Dashboard Backround/` | Power BI dashboard layout/background templates (Pages 1–3). |

---

## 🧰 Tech Stack

- **Python** — `pandas`, `numpy`
- **Visualization** — `matplotlib`, `seaborn`, `plotly` (choropleth map)
- **Notebook** — Jupyter / Google Colab
- **BI** — Microsoft Power BI

---

## 📊 Analyses Included

The notebook walks through 15 analyses, including:

1. Monthly sales trend over time
2. Monthly sales trend (all years combined)
3. Top 10 products by revenue
4. Top 10 products by average profit margin
5. Sales by channel (pie chart)
6. Average Order Value (AOV) distribution
7. Profit margin % vs. unit price
8. Unit price distribution per product
9. Total sales by US region
10. Total sales by state (choropleth map)
11. Top 10 states by revenue and order count
12. Average profit margin by channel
13. Top and bottom 10 customers by revenue
14. Customer segmentation: revenue vs. profit margin
15. Correlation heatmap of numeric features

---

## 🔍 Key Insights

- **Monthly Revenue Cycle:** Revenue stays stable between ≈\$23M–\$26.5M across 2014–2017, with no consistent seasonal spikes. The sharpest drop (≈\$21.2M) occurs in early 2017, indicating a possible one-time disruption.
- **Channel Mix:** Wholesale 54%, Distributors 31%, Exports 15% — a clear opportunity to scale international presence.
- **Top Products (Revenue):** Product 26 (\$118M), Product 25 (\$110M), Product 13 (\$78M); mid-tier \$68–75M; bottom performers \$52–57M.
- **Profit Margins:** Range broadly from ≈18% to ≈60% with no strong correlation to unit price, suggesting standardized pricing across tiers.
- **Seasonal Volume:** No strong monthly pattern, but a slight uptick around May–June.
- **Regional Performance:** California leads with ≈\$230M revenue and 7,500+ orders; Illinois/Florida/Texas ≈\$85M–\$110M; NY/Indiana ≈\$54M.

---

## 💡 Recommendations

1. **Outlier Strategy:** Exclude or formalize bulk-order and promotional SKUs when calculating averages.
2. **Margin Uplift:** Apply top-product pricing levers to mid/low tiers; cut costs on underperformers.
3. **Export Growth:** Invest in targeted overseas marketing and distributor partnerships.
4. **Seasonal Planning:** Shift spend toward the January trough and May–June peak; investigate the 2017 anomaly.
5. **Dashboard Prep:** Maintain aggregated tables for time series, channel mix, and product performance in Power BI.

---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/usa-regional-sales-analysis.git
   cd usa-regional-sales-analysis
   ```
2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn plotly openpyxl jupyter
   ```
3. Launch the notebook:
   ```bash
   jupyter notebook EDA_Regional_Sales_Analysis.ipynb
   ```
   > Note: the notebook's data-loading cell originally mounts Google Drive (Colab). To run locally, point `pd.read_excel(...)` at the included `Regional Sales Dataset.xlsx`.
4. Open `SALES REPORT.pbix` in **Power BI Desktop** to explore the interactive dashboard.

---

## 📌 Note

Data is for a fictional company ("Acme Co.") and is used here for educational and portfolio purposes.
