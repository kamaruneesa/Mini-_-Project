# Mini-_-Project# DATAGO Global Supply Chain Insights & Logistics Analysis

## 📌 Project Overview
An end-to-end data analytics project examining global supply chain operations, shipping performance, order profitability, and delivery bottlenecks using the **DATAGO Global Supply Chain** dataset. The goal of this analysis is to uncover operational inefficiencies and provide data-driven recommendations to improve on-time delivery and profit margins.

---

## 🎯 Business Problem & Objectives
Global supply chains often struggle with unpredictable shipping delays, rising fulfillment costs, and regional bottlenecks. This project aims to answer the following key business questions:
* What is the overall on-time delivery rate vs. late delivery risk across different shipping modes?
* Which regions, markets, and product categories generate the highest revenue and profit margins?
* What are the primary drivers behind shipment delays and order cancellations?
* How can logistics strategies be optimized to reduce transit times and improve customer satisfaction?

---

## 🛠️ Tools & Technologies Used
* **Data Cleaning & Transformation:** [e.g., Microsoft Excel / Power Query / SQL]
* **Data Modeling & Calculations:** [e.g., DAX (Data Analysis Expressions)]
* **Data Visualization:** [e.g., Microsoft Power BI / Tableau]
* **Version Control:** Git & GitHub

---

## 📂 Dataset Description
The dataset comprises **[insert total number of rows, e.g., 180,000+]** transactional records and **[insert number of columns, e.g., 53]** attributes covering order details, customer demographics, shipping schedules, and financial metrics.

* **Key Features Analyzed:**
  * `Order Date` & `Shipping Date` (Real vs. Scheduled days for shipment)
  * `Shipping Mode` (Standard Class, First Class, Second Class, Same Day)
  * `Delivery Status` (Advance Shipping, Shipping on Time, Late Delivery, Shipping Canceled)
  * `Market` & `Order Region` (Global geographic breakdown)
  * `Category Name`, `Sales`, & `Order Profit Per Order`

---

## 🧹 Data Cleaning & Preparation
Before building the dashboard, the raw data underwent the following preparation steps:
1. **Handling Missing & Irrelevant Data:** Removed duplicate entries, standardized null values, and dropped non-analytical columns (such as customer passwords/emails).
2. **Data Type Standardization:** Formatted date columns (`Order Date`, `Shipping Date`) and currency fields for accurate time-intelligence and financial calculations.
3. **Feature Engineering (DAX / Calculated Columns):**
   * Created variance metrics comparing `Days for shipping (real)` against `Days for shipment (scheduled)`.
   * Built KPI measures for **Total Sales**, **Total Profit**, **Profit Margin %**, **Total Orders**, and **Late Delivery Rate %**.
4. **Data Optimization:** [Optional: Mention if you filtered specific years or optimized the data model for performance].

---

## 💡 Key Insights & Findings
* **Delivery Performance:** **[X%]** of total orders experienced late deliveries, with **[e.g., Standard Class / First Class]** accounting for the highest volume of delayed shipments.
* **Regional Trends:** **[Insert Top Market/Region, e.g., Western Europe / LATAM]** generated the highest sales volume, whereas **[Insert Region]** showed the highest rate of shipping delays.
* **Product Profitability:** **[Insert Top Category, e.g., Fishing / Cleats]** led overall revenue, while certain high-discount orders resulted in negative profit margins.
* **Shipping Mode Trade-offs:** While **Same Day** and **First Class** offer faster transit, tighter scheduling windows led to a higher percentage of missed delivery targets compared to **Standard Class**.

---

## 📊 Dashboard Preview
*(Replace the image path below with the screenshot uploaded to your GitHub repository)*

![Supply Chain Dashboard Overview](images/dashboard_overview.png)

---

## 🚀 Strategic Recommendations
1. **Optimize Shipping Schedules:** Adjust scheduled delivery estimates for **[Specific Shipping Mode]** in high-delay regions to set realistic customer expectations and reduce late-delivery penalties.
2. **Focus on High-Margin Categories:** Re-evaluate discounting strategies on **[Low-Margin Category]** where high promotional discounts are eroding net profitability.
3. **Regional Logistics Review:** Partner with alternative regional carriers in **[High-Delay Region]** to resolve recurring customs and transit bottlenecks.

---

## 💻 How to Use This Repository
1. Clone this repository to your local machine:
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
         




