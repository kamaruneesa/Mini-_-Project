# Project Title: Supply Chain, Sales & Delivery Performance Analytics


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
* > **Note:** For focused analysis and performance optimization, the dataset was scoped to **2,000 rows** (`2K` total orders) for this dashboard

---

## 🧹 Data Cleaning & Transformation
1. **Remove Duplicate**
2. **Data Type Formatting:**
3. **Remove Unnecessary Column**
   -  Home tab  ➡️ Remove Column
        - Order Zip code  (97% null)
        - Customer Password (Not given)
        - Customer Email (NOT)

4. **check Blank Valus**
5. **Final Data Quality check**
---
##  📱* **Data Modeling & Calculations:**

1. **min_date:min_date =** MIN(DataCoSupplyChainDataset3[order date (DateOrders)])
2. **max_ date=**max_date = MAX(DataCoSupplyChainDataset3[order date (DateOrders)])
3. **Date_Table =** ADDCOLUMNS(CALENDAR(DATE(2015,01,06) , DATE(2018,01,31)) ,"year", YEAR([DATE]), "Month Number" ,MONTH([DATE]),"Month Name", FORMAT([DATE],"MMMM"),"QUARTER","Q" &  QUARTER([DATE]), "Day" ,DAY([Date]) ,"Day Name" , FORMAT([Date],"DDDD"))
4. **Total Orders =** COUNT(DataCoSupplyChainDataset3[Order Id])
5. **Total Profit =** SUM(DataCoSupplyChainDataset3[Order Profit Per Order])
6. **Total Sales =** SUM(DataCoSupplyChainDataset3[Sales])
7. **Profit Margin % =** DIVIDE([Total Profit], [Total Sales], 0)
8. **Late Delivery Rate % =** DIVIDE(CALCULATE(COUNT(DataCoSupplyChainDataset3[Delivery Status]),DataCoSupplyChainDataset3[Delivery Status]= "Late delivery"),COUNT(DataCoSupplyChainDataset3[Delivery Status]),0)
---
### 🔗 Data Modeling & Relationships (Star Schema)

| Fact Table | Dimension Table | Linking Columns | Cardinality | Cross-Filter Direction |
| :--- | :--- | :--- | :--- | :--- | 
| `DataCoSupplyChainDataset3` | `Date_Table` | `order date` ➡️ `Date` | Many-to-one (`*:1`) | Single | 
| `tokenized_access_logs1` | `Date_Table` | `Date` ➡️ `Date` | Many-to-one (`*:1`) | Single | 


---
### 📊 Key Executive Insights

* **High Late Delivery Rate:** Nearly half of all orders (**49.90%**) experience delivery delays, indicating a critical bottleneck in logistics.
* **Strong Financial Performance:** Generated **$483.57K** in total sales and **$48.27K** in profit (~10% margin) across **2K** total orders.
* **Top Revenue Drivers:** The **Consumer** segment and departments like **Fan Shop** and **Apparel** contribute the highest share of sales.

---


### 📊 Dashboard Visuals & Components

| Visual Type | Title / Metric | Description |
| :--- | :--- | :--- |
| **KPI Cards** | Late Delivery Rate %, Total Orders, Total Profit, Total Sales | Highlights core business and logistics metrics at a glance. |
| **Clustered Column Chart** | Total Profit & Total Sales by Year | Compares yearly revenue and profit performance trend. |
| **Donut Charts** | Sum of Sales by Department Name & Customer Segment | Illustrates revenue breakdown across different product departments and customer group. |
| **Horizontal Bar Chart** | Count of Delivery Status | Displays the volume of orders across various delivery states (e.g., Late delivery, Advance shipping). |
| **Slicers / Filters** | Customer Segment, Department Name, Delivery Status | Enables interactive filtering for dynamic data analysis. |

---

         




