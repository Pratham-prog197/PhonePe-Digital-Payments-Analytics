# 📱 PhonePe Digital Payments Analytics
### End-to-End Data Analysis & Business Intelligence Project | Python • Pandas • NumPy • Power BI • DAX

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)

---

## 📌 Project Overview

Digital payments have become an integral part of India's financial ecosystem. Understanding transaction behaviour, regional performance, customer adoption and engagement is increasingly important for digital payment platforms.

This project focuses on analysing **PhonePe Pulse data from Q1 2018 to Q2 2021** to identify patterns in digital payment activity across Indian states and districts.

The project follows an end-to-end analytics approach, beginning with raw data exploration and preprocessing using Python, followed by exploratory and advanced analysis, and concluding with an interactive Power BI reporting solution.

The analysis explores transaction trends, transaction values, payment preferences, registered users, app activity, device-brand distribution and demographic relationships.

The final objective is to transform raw data into meaningful business insights that can support regional performance evaluation and data-driven decision-making.

---

## 🎯 Business Problem

Digital payment platforms need to understand how transaction activity and user adoption vary across different geographical regions and over time.

Monitoring total transaction volume alone is not sufficient. Businesses also need to understand regional performance, user engagement, payment preferences and the relationship between demographic characteristics and digital payment activity.

This project addresses the following business questions:

1. How has digital payment activity evolved over the available period?
2. Which states and districts demonstrate higher or lower transaction activity?
3. How does transaction value vary across different regions?
4. What are the most frequently leading transaction categories?
5. How do registered users and app activity relate to transaction behaviour?
6. Which device brands account for larger registered-user counts?
7. Are demographic indicators such as population density associated with regional transaction activity?
8. What opportunities can be identified for further investigation into digital payment adoption?

### Business Objective

To analyse transaction performance, user engagement and regional adoption patterns, identify meaningful trends and potential opportunities, and communicate the findings through an interactive business intelligence dashboard.

---

## 🎯 Project Objectives

- Understand and prepare multiple raw datasets for reliable analysis.
- Perform data profiling, cleaning and preprocessing using Python.
- Conduct exploratory data analysis to identify transaction patterns.
- Analyse yearly and quarterly transaction trends.
- Compare state-level and district-level transaction performance.
- Investigate transaction categories and payment preferences.
- Examine registered-user distribution and app activity.
- Analyse device-brand distribution across regions.
- Explore relationships between demographic indicators and transaction metrics.
- Validate consistency between state-level and district-level aggregations.
- Develop an interactive Power BI dashboard.
- Translate analytical findings into business insights and recommendations.

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Python | Data analysis and processing |
| Pandas | Data cleaning, transformation, aggregation and merging |
| NumPy | Numerical operations and statistical calculations |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization and correlation analysis |
| Jupyter Notebook | Interactive analysis and documentation |
| Power BI | Interactive dashboard development |
| DAX | Measures, KPIs and dynamic calculations |
| Microsoft Excel | Raw dataset inspection and storage |

---

## 📂 Dataset Description

The analysis uses five core datasets from the PhonePe Pulse workbook, covering state-level, district-level, transaction, user, device and demographic information.

**Analysis Period:** Q1 2018 – Q2 2021

| Dataset | Description | Analytical Purpose |
|---|---|---|
| State_Txn and Users | State-level transactions, transaction amount, registered users and app opens | Transaction trends and user activity |
| State_TxnSplit | Transaction categories and corresponding metrics | Payment-category analysis |
| State_DeviceData | Device brands and registered-user metrics | Device-brand analysis |
| District_Txn and Users | District-level transaction and user metrics | Regional performance analysis |
| District Demographics | District population, area, density and supporting geographical information | Demographic analysis |

### Key Data Dimensions

The datasets contain information related to:

- State
- District
- Year
- Quarter
- Transaction Type
- Transaction Count
- Transaction Amount
- Average Transaction Value
- Registered Users
- App Opens
- Device Brand
- Population
- Area
- Population Density

---

## 🔍 Project Workflow

### 1. Data Understanding and Exploration

The first stage involved loading the Excel workbook into Python and examining the structure of each dataset.

Activities performed:

- Loaded the individual worksheets into Pandas DataFrames.
- Examined dataset dimensions and column names.
- Inspected data types and descriptive statistics.
- Reviewed numerical distributions.
- Investigated the structure and relationships between datasets.

**Objective:** Understand the available data and identify potential data-quality issues before beginning the analysis.

### 2. Data Cleaning and Preprocessing

Performed preprocessing operations to improve data consistency and prepare the datasets for analysis.

Activities performed:

- Identified missing values and calculated missing-value percentages.
- Investigated missing transaction amounts and average transaction values.
- Checked exact duplicate records.
- Investigated invalid and negative numerical values.
- Standardized text fields such as State, District and Brand.
- Validated numerical data types.
- Investigated missing district codes and applied district-code mappings.
- Prepared datasets for subsequent analysis.

**Objective:** Improve data consistency and reduce the risk of misleading analytical results.

### 3. Exploratory Data Analysis (EDA)

Performed exploratory analysis to understand transaction behaviour and regional differences.

Key analytical areas:

**Transaction Analysis**
- Yearly transaction volume.
- Quarterly transaction trends.
- Total transaction amount.
- Average transaction value.
- Top and bottom performing states.
- Cumulative transaction activity.

**Transaction Category Analysis**
- Distribution of transaction types.
- Most frequently leading transaction categories.
- State-wise transaction preferences.
- Transaction mix analysis for selected regions.

**User Analysis**
- Registered-user distribution.
- Quarterly app activity.
- State-wise user comparisons.
- Relationship between app opens and transaction activity.

**Device Analysis**
- Registered users by device brand.
- Device-brand distribution across states.
- Comparison of device-brand user metrics.

**Regional Analysis**
- State-level transaction performance.
- District-level transaction performance.
- Population distribution.
- Regional differences in transaction activity.

### 4. Advanced Analysis and Dataset Integration

Beyond basic exploratory analysis, additional analysis was performed by combining datasets and creating derived metrics.

**A. Registered Users vs Population**

Compared registered-user counts with population data to calculate a user-to-population ratio.

Formula:

`User Penetration Ratio = (Registered Users / Population) × 100`

This provides additional context for comparing regions with different population sizes.

**B. Population Density vs Transaction Volume**

Combined district-level transaction information with demographic data to investigate the relationship between population density and transaction volume.

Pearson correlation was used to examine the strength and direction of the linear relationship.

**C. Transaction Amount per Registered User**

Calculated transaction amount relative to registered users to provide another perspective on regional transaction performance.

**D. Device-Brand Usage Ratio**

Combined device-brand and state-level user information to compare the relative representation of device brands across states.

**E. State–District Reconciliation**

Aggregated district-level transaction metrics by state and compared them with the corresponding state-level metrics.

This exercise helped identify discrepancies requiring further investigation before using the affected figures for reporting.

### 5. Data Visualization

Used Matplotlib and Seaborn to communicate analytical findings through visual representations.

The visualizations covered:

- Yearly and quarterly transaction trends.
- State-wise transaction comparisons.
- Transaction-category distribution.
- Device-brand analysis.
- District population distribution.
- Population density versus transaction volume.
- User and app activity relationships.
- Correlation analysis.

### 6. Power BI Dashboard Development

After completing the Python analysis, an interactive six-page Power BI report was developed.

The report combines key performance indicators, analytical visualizations, regional comparisons and business recommendations.

---

## 📊 Power BI Dashboard

The Power BI report contains six analytical pages designed to provide different perspectives on digital payment performance.

### Page 1 — Executive Overview

Provides a high-level summary of digital payment performance.

Key components:

- Total Transactions
- Total Transaction Value
- Average Transaction Value
- Latest Registered Users
- Total App Opens
- Transaction-type distribution
- Transaction volume trend
- Transaction value trend
- Top states by transaction volume
- Dynamic transaction metric selection

**Purpose:** Provide an executive-level overview of overall transaction performance.

#### Dashboard Preview

<img width="1397" height="790" alt="Screenshot 2026-11-07 002425" src="https://github.com/user-attachments/assets/de98b7c0-7c13-4b64-b608-279d6c148b60" />

---

### Page 2 — Transaction Trends & Growth

Focuses on understanding how transaction activity changes over time.

Key components:

- Quarterly transaction volume
- Quarterly transaction value
- Quarter-over-quarter growth
- Cumulative transactions
- Top states by transaction volume
- Transaction performance KPIs

**Purpose:** Identify transaction growth patterns, changes in activity and regional performance over the reporting period.

#### Dashboard Preview
<img width="1391" height="790" alt="Screenshot 2026-11-07 002536" src="https://github.com/user-attachments/assets/482366cd-de85-4e93-ae0a-79cc49063d6d" />


---

### Page 3 — User Adoption & Device Analysis

Explores registered-user metrics, app activity and device-brand distribution.

Key components:

- Latest Registered Users
- Average Registered Users per State
- Total Transactions
- Total App Opens
- Registered-user growth
- Quarterly app opens
- Device-brand distribution
- Device metrics by brand
- State-wise registered-user comparison

**Purpose:** Understand user-registration patterns, app activity and device-brand representation.

#### Dashboard Preview
<img width="1392" height="790" alt="Screenshot 2026-11-07 002600" src="https://github.com/user-attachments/assets/9cc09019-fdd7-4b6c-a980-8f38bad40620" />

---

### Page 4 — State & District Performance

Provides a geographical comparison of transaction performance across Indian states and districts.

Key components:

- Top states by transaction volume
- Top states by transaction value
- Top districts by transaction volume
- Top districts by transaction amount
- Average transaction value
- District-level performance details

**Purpose:** Identify geographical differences in transaction activity and compare regional performance at different levels.

#### Dashboard Preview
<img width="1392" height="791" alt="Screenshot 2026-11-07 002621" src="https://github.com/user-attachments/assets/cd2a4a22-00b5-425d-aa4f-c8b5b883266a" />

---

### Page 5 — Insights & Recommendations

Brings together important analytical findings and regional comparisons.

Key components:

- State contribution to total transactions
- Transaction volume versus transaction value
- Transactions per app open
- Transaction KPIs
- Regional performance comparisons
- Analytical insight summaries

**Purpose:** Translate dashboard metrics into business-oriented observations and identify areas for further investigation.

#### Dashboard Preview


<img width="1390" height="790" alt="Screenshot 2026-11-07 002653" src="https://github.com/user-attachments/assets/b86d5485-9cd5-4a6e-94b8-b816174dacdc" />

---

### Page 6 — Final Insights

Presents the final business recommendations in a structured format.

Key components:

- Insight Area
- Observation
- Priority
- Recommended Action
- Status

**Purpose:** Connect analytical findings with potential business actions and areas requiring further investigation.

#### Dashboard Preview

<img width="1390" height="790" alt="Screenshot 2026-11-07 002727" src="https://github.com/user-attachments/assets/8488e10b-147c-491f-9f92-1a5e31a8342d" />


---

## 📈 Key Findings and Insights

The following findings were derived from the analysis of the available datasets.

### 1. Significant Growth in Digital Payment Activity

Total transaction volume increased from approximately **1.08 billion in 2018 to 7.97 billion in 2020**.

This indicates substantial growth in digital payment activity across the analysed period.

*Note: 2021 contains only the first two quarters and should not be compared directly with full-year totals.*

### 2. Leading States by Transaction Volume

Karnataka, Maharashtra and Telangana recorded the highest cumulative transaction volumes in the analysis.

This highlights differences in regional digital payment activity. Absolute transaction totals should also be interpreted alongside population and user-base differences.

### 3. Transaction Category Preferences

Peer-to-peer payments were the leading transaction category in approximately **61.7% of state-quarter combinations**.

Recharge and bill payments were the leading category in approximately **32.1% of state-quarter combinations**.

These figures represent the frequency with which each category ranked first, not its share of all transactions.

### 4. Delhi Transaction Mix

In Delhi during Q3 2019:

- Merchant payments accounted for approximately 42.4% of transactions.
- Peer-to-peer payments accounted for approximately 36.2%.

Together, these categories represented approximately **78.6% of transactions** in that period.

### 5. Relationship Between Transaction Amount and Volume

Transaction count and transaction amount showed a strong positive correlation of approximately **0.98**.

This indicates that higher transaction counts were strongly associated with higher total transaction amounts in the analysed data.

### 6. App Activity and Transaction Behaviour

App opens and transaction activity showed a positive correlation of approximately **0.84**.

This suggests an association between higher app activity and higher transaction activity, although correlation does not establish causation.

### 7. Population Density and Transaction Activity

Population density and transaction volume showed a weak positive correlation of approximately **0.19**.

This suggests that population density alone was not a strong indicator of transaction activity in the analysed data.

### 8. State–District Data Reconciliation

The reconciliation analysis identified a discrepancy in Andhra Pradesh's transaction amount:

| Reporting Level | Approximate Transaction Amount |
|---|---:|
| State-level dataset | ₹3.19 trillion |
| Aggregated district-level dataset | ₹3.86 trillion |

This discrepancy requires further investigation into reporting periods, aggregation logic, missing records and potential duplicate data.

---

## 💡 Business Recommendations

Based on the analytical findings, the following recommendations were identified.

| Business Area | Observation | Recommended Action |
|---|---|---|
| Regional Performance | Karnataka, Maharashtra and Telangana recorded high transaction volumes | Prioritize reliable payment processing and customer retention in established high-volume markets |
| User Engagement | User registration and transaction activity vary across regions | Investigate regions with relatively large registered-user bases but lower transaction activity |
| Merchant Payments | Merchant payments represented a significant share of Delhi's transaction mix in Q3 2019 | Investigate merchant acceptance and payment frequency to identify opportunities |
| Data Quality | State-level and district-level figures showed a discrepancy | Reconcile reporting periods, aggregation logic and missing records before reporting |
| Market Evaluation | Regional transaction activity differs across states | Evaluate transaction volume, registered-user penetration and demographic metrics together |
| Performance Monitoring | Transaction activity changes over time | Monitor quarterly transaction counts, values and transaction-type mix |

These recommendations represent potential business actions suggested by the available analysis. Their effectiveness would need to be evaluated using additional operational and customer-level information.

---

## 📁 Repository Structure

The project repository is organised as follows:

```text
PhonePe-Digital-Payments-Analytics/
│
├── data/
│   └── phonepe_raw_data.xlsx
│
├── notebooks/
│   └── PhonePe_Data_Analysis.ipynb
│
├── powerbi/
│   └── PhonePe_Dashboard.pbix
│
├── images/
│   ├── 01_executive_overview.png
│   ├── 02_transaction_trends.png
│   ├── 03_user_device_analysis.png
│   ├── 04_state_district_performance.png
│   ├── 05_insights_recommendations.png
│   └── 06_final_insights.png
│
├── README.md

```

---




### 6. Explore the Power BI Dashboard

Open:

`powerbi/PhonePe_Dashboard.pbix`

Use the report filters to explore transaction trends, state performance, user metrics and device-brand analysis.

---

## 📦 Python Dependencies

The required Python libraries are listed below:

```text
pandas
numpy
matplotlib
seaborn
openpyxl
jupyter
```


---



## 🧠 Skills Demonstrated

**Technical Skills**
- Python
- Pandas and NumPy
- Data Cleaning and Preprocessing
- Exploratory Data Analysis
- Data Aggregation and Transformation
- Dataset Merging and Validation
- Correlation Analysis
- Data Visualization
- Power BI
- DAX
- Interactive Dashboard Development

**Analytical Skills**
- Business Problem Understanding
- Transaction Trend Analysis
- Regional Performance Analysis
- User Engagement Analysis
- Demographic Analysis
- Data Quality Assessment
- Business Insight Generation
- Data-Driven Recommendations

---

## 👨‍💻 Author

**Pratham Pulkeet**

B.Tech Student | Aspiring Data Analyst

Technical Interests: Python, SQL, Power BI, Data Analytics and Business Intelligence.

---

## ⭐ Acknowledgement

This project uses PhonePe Pulse data for educational and analytical purposes.

The analysis is intended to demonstrate practical data analytics and business intelligence skills through a real-world digital payments use case.

If you find this project useful, feel free to ⭐ the repository.

