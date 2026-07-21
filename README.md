# Forecasting Financial Inclusion in Ethiopia

## Project Overview

This project aims to build a forecasting system that analyzes and predicts Ethiopia's financial inclusion using time series analysis. The focus is on forecasting two key financial inclusion indicators defined by the World Bank Global Findex framework:

* **Access** – Account Ownership Rate
* **Usage** – Digital Payment Adoption Rate

The project explores historical financial inclusion trends, identifies the impact of major policy and market events, enriches the dataset with additional explanatory variables, and prepares the data for forecasting future financial inclusion outcomes.

---

# Objectives

The project seeks to answer the following questions:

* What factors drive financial inclusion in Ethiopia?
* How have major events such as Telebirr, M-Pesa, and national policy reforms influenced financial inclusion?
* How is financial inclusion expected to evolve in 2025, 2026, and 2027?

---

# Dataset

The primary dataset (`ethiopia_fi_unified_data`) contains four record types:

* **Observation** – Historical measurements of financial inclusion and related indicators.
* **Event** – Major policy changes, product launches, infrastructure developments, and market milestones.
* **Target** – Official policy goals and future targets.
* **Impact Links** – (Planned for later stages) Relationships between events and financial inclusion indicators.

Supporting files include:

* `reference_codes.csv`
* `README.md`
* Additional Data Enrichment Guide

---

# Work Completed

## 1. Data Understanding

The dataset structure was explored to understand:

* Dataset dimensions and schema
* Data types
* Missing values
* Record types
* Financial inclusion pillars
* Indicator codes
* Source types
* Confidence levels
* Temporal coverage
* Event timeline

The dataset contains:

* Historical financial inclusion observations
* Major digital finance events
* Official policy targets

---

## 2. Exploratory Data Analysis (EDA)

Initial exploration included:

* Dataset overview (`info()`)
* Missing value assessment
* Frequency analysis of categorical variables
* Distribution of record types
* Indicator inventory
* Event chronology
* Temporal coverage analysis

These steps helped identify areas requiring enrichment before forecasting.

---

## 3. Dataset Enrichment

The enrichment process was initiated to improve forecasting capability.

### Completed

One new explanatory indicator has been added:

**Internet Penetration**

Source:

* World Bank Open Data
* Indicator: *Individuals using the Internet (% of population)* (`IT.NET.USER.ZS`)

Years Added:

* 2020
* 2021
* 2022
* 2023
* 2024

Reason for inclusion:

Internet penetration is considered a leading indicator of digital payment adoption because increased internet access enables greater use of mobile banking, digital wallets, and other digital financial services.

---

# Planned Enrichment

Additional indicators planned for enrichment include:

* Mobile Cellular Subscriptions
* Smartphone Penetration
* Active Mobile Money Accounts
* Agent Network Size

These indicators were selected because they are expected to improve forecasting performance by providing explanatory variables related to Ethiopia's digital financial ecosystem.

---

# Current Project Status

Completed:

* Dataset loading
* Data understanding
* Initial exploratory analysis
* Dataset quality assessment
* Internet Penetration enrichment

In Progress:

* Additional data enrichment
* Documentation of enrichment sources

Planned:

* Event-impact modeling
* Time series forecasting
* Forecast evaluation
* Visualization dashboard
* Final report

---

# Tools and Libraries

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn (planned)
* Statsmodels (planned)
* Prophet (planned)
* Jupyter Notebook

---

# Data Sources

* World Bank Open Data
* National Bank of Ethiopia
* GSMA Mobile Money Reports
* International Telecommunication Union (ITU)
* Ethiopia financial sector reports

---

# Next Steps

The next phase of the project will focus on:

1. Completing dataset enrichment.
2. Building relationships between events and financial inclusion indicators.
3. Developing forecasting models for Access and Usage indicators.
4. Evaluating model performance.
5. Forecasting Ethiopia's financial inclusion for 2025–2027.
