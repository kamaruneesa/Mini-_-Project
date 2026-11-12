# Project Title: Supply Chain, Sales & Delivery Performance Analytics

## 📌 Project Overview
An end-to-end big data analytics project utilizing the **DataCo Supply Chain for Big Data Analysis** dataset to thoroughly examine global logistics operations, sales performance, and delivery efficiency[cite: 1]. This project focuses on processing large-scale supply chain data to evaluate key operational metrics, including **Sales & Profit Analysis**, **Delivery & Late Delivery Performance**, **Product Category breakdown**, **Customer Segmentation**, **Shipping Mode efficiency**, and **Regional variations**[cite: 1]. The primary goal is to uncover complex supply chain bottlenecks, optimize fulfillment processes, and deliver actionable data-driven insights.

---

## 🔍 ഇതിൽ ചെയ്യാൻ കഴിയുന്നത് (Key Objectives & Scope)[cite: 1]
* **Sales & Profit Analysis:** Evaluate total revenue, profit margins, and financial performance across different product categories and markets[cite: 1].
* **Delivery Performance:** Analyze scheduled vs. real shipping days to track on-time fulfillment rates[cite: 1].
* **Late Delivery Analysis:** Identify the primary root causes and patterns behind delayed shipments and high-risk orders[cite: 1].
* **Product Category Analysis:** Discover which product lines drive the highest sales volume versus those facing high return or delay rates[cite: 1].
* **Customer Segmentation:** Understand customer purchasing behaviors and regional demand patterns[cite: 1].
* **Shipping Mode Analysis:** Compare delivery efficiencies across different shipping classes (Standard, First Class, Same Day, etc.)[cite: 1].
* **Regional Performance:** Assess global regional bottlenecks and fulfillment efficiency[cite: 1].

---

## 🛠️ Tools & Technologies Used
* **Data Cleaning & Preparation:** Microsoft Excel 
* **Data Modeling & Calculations:** DAX (Data Analysis Expressions)
* **Data Visualization:** Microsoft Power BI 
* **Version Control:** Git & GitHub

---

## 📂 Dataset Source
* **Dataset Name:** https://www.kaggle.com/datasets/shashwatwork/dataco-smart-supply-chain-for-big-data-analysis?select=DataCoSupplyChainDataset.csv 
* **Platform:** Kaggle

---

## 🧹 Data Cleaning & Transformation
1. **Remove Duplicate**
2. **Data Type Formatting:**
3. **Remove Unnecessary Column**
   -  Home tab  ➡️ Remove Column
        - Order Zip code  (97% null)
        - Customer Password (Not given)
        - Customer Email (NOT)

4.**check Blank Valus**
5. **Final Data Quality check**
---
##  📱* **Data Modeling & Calculations:**

## 💡 Key Insights & Findings
* **Delivery Risks:** Certain shipping modes experience higher rates of late deliveries due to tight transit windows.
* **Regional Bottlenecks:** Specific regions face longer transit times, impacting overall customer satisfaction.
* **Profitability Drivers:** High-performing product categories contribute the majority of the profit margins.

---

## 📊 Dashboard Preview
*(Replace the image path below with your dashboard screenshot)*
![Supply Chain Dashboard](images/dashboard_preview.png)

---

## 💻 How to Use This Repository
1. Clone the repository:
   ```bash
   git clone [https://github.com/](https://github.com/)[Your-Username]/[Your-Repository-Name].git
# DATACO GLOBAL SUPPLY CHAIN INSIGHTS 
## Title: DATACO GLOBAL SUPPLY CHAIN INSIGHTS
## Source: Kaggle- DataCo Supply Chain Dataset
   **Dataset LInk:https://www.kaggle.com/datasets/shashwatwork/dataco-smart-supply-chain-for-big-data-analysis?select=DataCoSupplyChainDataset.csv**
## T00LS
 **Data Cleaning & Preparation**
  - Excel & Power Query



**Excel-Import**
 - Excel ➡️ Blank Workbook ➡️Form File ➡️FROM Text /csv➡️ Select File ➡️Import➡️Transform data ➡️
 - Import next files ➡️ Power Query Editor ➡️ Data Tab ➡️ Get DATA ➡️Form File ➡️FROM Text /csv➡️ Select File ➡️Import➡️Transform data ➡️

## Data Cleaning##

**Remove Duplicate**
 - select column "order item id " ➡️ home tab  ➡️ Remove Row ➡️Remove Duplicates

**Remove Unnecessary Column**
   -  Home tab  ➡️ Remove Column
        - Order Zip code  (97% null)
        - Customer Password (Not given)
        - Customer Email (NOT)
    
**Correct Data Type**
   - Oder Date ➡️ Date
   - Shipping Date ➡️ Date

**Text column Cleaning**
  - Trim
  - Clean
  - Standardize category name
**check Blank Valus**
**Final Data Quality check**


## close & Lode 
         




