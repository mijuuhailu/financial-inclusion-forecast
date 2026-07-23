# Forecasting Financial Inclusion in Ethiopia

## Overview

This project develops a time series forecasting system to analyze and forecast Ethiopia's financial inclusion using the World Bank Global Findex framework. The focus is on predicting **Account Ownership (Access)** while incorporating key digital finance events and supporting indicators.

---

## Project Progress

### 1. Data Understanding
- Explored the unified dataset structure.
- Analyzed record types, indicators, pillars, and data sources.
- Identified missing values and data limitations.
- Examined the timeline of major financial inclusion events.

### 2. Exploratory Data Analysis (EDA)
- Visualized historical Account Ownership trends.
- Explored indicator distributions and event chronology.
- Identified that the target variable has only four historical observations (2014, 2017, 2021, and 2024).

### 3. Data Enrichment
Added external indicators from trusted public sources (World Bank, ITU, and National Bank of Ethiopia):

- Internet Penetration (`USG_INTERNET_PEN`)
- Mobile Cellular Subscriptions (`USG_MOBILE_SUB`)
- Mobile Money Agent Network (`USG_AGENT_NETWORK`)
- Mobile Money Accounts (`USG_MM_ACCOUNTS`)
- Bank Branches (`USG_BANK_BRANCHES`)

### 4. Metadata Update
- Updated `reference_codes.csv` with the newly added indicator codes.
- Saved the enriched dataset as `ethiopia_fi_enriched.csv`.

### 5. Data Preparation
- Converted observation dates to yearly format.
- Built a modeling dataset using annual observations.
- Created intervention variables for:
  - Telebirr launch
  - M-Pesa launch
  - Fayda rollout
- Interpolated missing yearly Account Ownership values while preserving original observations.

### 6. Forecasting
- Developed a baseline time series forecasting model.
- Forecasted Ethiopia's Account Ownership Rate for:
  - 2025
  - 2026
  - 2027

### 7. Visualization
Generated visualizations for:
- Historical Account Ownership trend
- Forecasted Account Ownership (2025–2027)
- Normalized comparison of financial inclusion indicators

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Jupyter Notebook