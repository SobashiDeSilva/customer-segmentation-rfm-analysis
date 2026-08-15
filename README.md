# Customer Segmentation using RFM Analysis

## Overview
This project segments customers of an online retail business using **RFM analysis** (Recency, Frequency, Monetary) to identify high-value customers and prioritize marketing/retention efforts. Built using Python for data processing and Power BI for business dashboarding.

## Business Question
Which customers should the business prioritize for retention marketing, and which segments offer the best return on re-engagement spend?

## Dataset
- **Source**: [UCI Online Retail Dataset](https://archive.ics.uci.edu/dataset/352/online+retail)
- ~540,000 transactions from a UK-based online retailer (Dec 2010 – Dec 2011)
- Cleaned to ~398,000 valid transactions after removing cancellations, missing customer IDs, and invalid entries

## Methodology
1. **Data Cleaning** (Python/Pandas) — removed cancelled orders, missing CustomerIDs, and negative quantities/prices
2. **RFM Calculation** — computed Recency, Frequency, and Monetary value per customer
3. **Scoring & Segmentation** — scored customers 1–4 on each RFM dimension using quartiles, combined into 5 business segments: Champions, Loyal Customers, At Risk, Lost, Potential Loyalist
4. **Dashboard** (Power BI) — built an interactive dashboard to visualize segment distribution, revenue contribution, and customer behavior patterns

## Key Findings
- **Champions** (30% of customers) generate **73% of total revenue** — a small core segment drives the majority of business value
- **At Risk** customers represent **$1.04M in historical revenue** — a high-ROI win-back opportunity before they become fully inactive
- **Lost** customers (29% of the base) contribute only 4% of revenue — low priority for retention spend

## Recommendations
- Protect and reward the Champions segment (loyalty perks, early access)
- Launch targeted win-back campaigns for At Risk customers
- Deprioritize retention spend on Lost customers; consider low-cost reactivation only
- Nurture Potential Loyalists and Loyal Customers toward Champion status

## Tools Used
- Python (Pandas, NumPy, Matplotlib, Seaborn) — data cleaning & RFM calculation
- Power BI — interactive business dashboard
- Jupyter/Google Colab — analysis environment

## Files in this Repository
- `RFM_Customer_Segmentation.ipynb` — full Python analysis notebook
- `rfm_segments.csv` — calculated RFM scores and segments per customer
- `RFM_Customer_Segmentation_Dashboard.pbix` — Power BI dashboard file
- `dashboard_screenshot.png` — dashboard preview

## Author
Sobashi | MIT Undergraduate, University of Kelaniya
