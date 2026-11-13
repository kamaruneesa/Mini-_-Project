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
7. **Late Delivery Rate % =** DIVIDE(CALCULATE(COUNT(DataCoSupplyChainDataset3[Delivery Status]),DataCoSupplyChainDataset3[Delivery Status]= "Late delivery"),COUNT(DataCoSupplyChainDataset3[Delivery Status]),0)
---
### 🔗 Data Modeling & Relationships (Star Schema)

| Fact Table | Dimension Table | Linking Columns | Cardinality | Cross-Filter Direction |
| :--- | :--- | :--- | :--- | :--- | :--- |
| `DataCoSupplyChainDataset3` | `Date_Table` | `order date` ➡️ `Date` | Many-to-one (`*:1`) | Single | 
| `tokenized_access_logs1` | `Date_Table` | `Date` ➡️ `Date` | Many-to-one (`*:1`) | Single | 


---

## 💡 Key Insights & Findings
* **Delivery Risks:** Certain shipping modes experience higher rates of late deliveries due to tight transit windows.
* **Regional Bottlenecks:** Specific regions face longer transit times, impacting overall customer satisfaction.
* **Profitability Drivers:** High-performing product categories contribute the majority of the profit margins.

---

## 📊 Dashboard Previe

---

         




