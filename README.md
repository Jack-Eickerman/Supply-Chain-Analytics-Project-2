# Supply-Chain-Analytics-Project-2
Analysis of Example Data as a Data Analyst in a Corporation
# Retail Supply Chain Optimization

**Assignment 2 – Supply Chain Analytics Project (SCAP)**  
Group Members: Jack and Shilpa

A comprehensive retail supply chain analysis project that includes data cleaning, exploratory analysis, hypothesis testing, demand forecasting, ABC inventory classification, reorder point calculation, and multi-criteria supplier evaluation.

Originally developed in Google Colab as a group assignment.

## Features & Key Analyses
- **Data Preprocessing** — Handling missing values (e.g., 212 in sales price, 75 in inventory stock), duplicates, data type fixes, no major outliers detected
- **EDA** — Monthly/weekly sales trends, revenue ranking by store, correlation heatmap (quantity sold vs. lead time, promo flag, delivery rate, defect rate, etc.)
- **Hypothesis Testing** (t-tests):
  - Promotion impact on sales (no significant difference, p > 0.05 across regions)
  - Perishable vs. non-perishable product sales (no significant difference)
- **Demand Forecasting** — Weighted Moving Average (WMA) model (weights [0.2, 0.3, 0.5]), evaluated with MAE, MSE, MAPE
  - Example: Detailed forecast for store S025
- **Inventory Optimization** — ABC classification based on two-year consumption value
  - A: ~54% of value (top priority)
  - B & C: Reduced via removal of low performers
  - Result: Improved revenue after reallocation
- **Reorder Point (ROP) & EOQ** — For product P0118 (includes safety stock at 95% service level, perishable flag consideration)
- **Supplier Evaluation & Ranking**:
  - Top cheapest suppliers (e.g., SUP09 lowest unit cost)
  - Best lead time (SUP01 ~2 days average)
  - Stacked performance (on-time delivery, defects, late deliveries)
  - Per-product/category best suppliers
