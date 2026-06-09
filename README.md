# Automobile Customer Segmentation & RFM Analysis

## 📌 Project Overview
This project focuses on conducting a **Customer Segmentation Analysis** for an automobile bike company using an **RFM (Recency, Frequency, Monetary) Model**. By analyzing historical transaction data, customers were segmented into 11 distinct behavior-based groups. 

The goal is to identify high-value customer segments and provide data-driven recommendations to optimize marketing strategies and boost sales revenue.

### 🛠️ Tech Stack & Tools
* **Data Quality & EDA:** Python 3.8 (Pandas, Matplotlib, Seaborn)
* **Business Intelligence & Dashboards:** Tableau
* **Environment:** Jupyter Notebooks

---
## 🎥 Dashboard Demo

![Dashboard Demo](images/dashboard_demo.gif)


## 📊 Dashboard & Analysis Preview

### Customer Age Distribution
![Age Distribution](images/age_distribution.png)

### Wealth Segmentation by Age Group
![Wealth Segmentation](images/wealth_segmentation.png)

### Car Ownership by State
![Car Ownership](images/car_ownership.png)

### Bike Purchases by Gender
![Gender Analysis](images/gender_analysis.png)

---

## 🔄 Project Workflow & Methodology

### 1. Data Quality Assessment (DQA) & Cleaning
Raw data from 4 distinct sources (`Transactions`, `NewCustomerList`, `CustomerDemographic`, and `CustomerAddress`) underwent rigorous preprocessing:
* **Inconsistency Resolution:** Standardized mismatched categories (e.g., `Gender` and `State` fields).
* **Missing & Outlier Handling:** Imputed or dropped missing data based on volume; filtered out age outliers.
* **Feature Engineering:** Transformed raw dates to create `Age`, `Age Group`, and `Profit` (List Price - Standard Price) metrics.

### 2. Exploratory Data Analysis (EDA)
Key behavioral insights discovered during analysis:
* **Age Demographics:** Both new and existing customer bases peak between **40–49 years old**. 
* **Gender Split:** Bike purchases are relatively even, with females accounting for **51%** of total transactions.
* **Industry Drivers:** The **Manufacturing** and **Financial Services** sectors yield the highest density of customers (~20% each).
* **Wealth Categories:** "Mass Customers" form the largest segment across all age groups.

### 3. RFM Modeling & Segmentation
Customers were scored based on Recency, Frequency, and Monetary values, then categorized into **11 segments** (including *Platinum, Very Loyal, Potential Loyalists, and At Risk*) to target marketing budgets efficiently.

> 📈 **Key Finding:** Scatter plot analysis validated that customers with lower recency (more recent purchases) and higher frequency correspond directly to higher monetary value and business revenue.

---

## 📂 Dataset Architecture
The project utilizes four primary data sheets containing Australian market data:
1.  **Transactions:** Purchase history, list prices, and standard prices.
2.  **Customer Demographics:** Age, gender, and job industry data.
3.  **Customer Address:** Regional distribution across Australian states.
4.  **New Customer List:** Potential target leads for future marketing campaigns.
