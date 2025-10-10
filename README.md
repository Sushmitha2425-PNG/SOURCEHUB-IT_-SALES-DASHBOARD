# 🏪 US Store Interactive Sales Dashboard  

### 📘 Overview  
This Power BI dashboard provides an **interactive overview of sales performance** for a US-based retail store.  
It enables exploration of total sales, profits, order distribution, and key performance insights across **time, products, and regions**.  

---

## 📊 Key Metrics  

| Metric | Value | Description |
|--------|--------|-------------|
| **Total Sales** | 742.00K | Total revenue generated from all transactions. |
| **Sum of Profit** | 18.45K | Total profit earned from all orders. |
| **Total Orders** | 1,764 | Count of unique customer orders. |
| **Average Order Value (AOV)** | 420.63 | Average revenue generated per order. |

---

## 🧮 DAX Measures Used  

```DAX
-- Total Sales
Total Sales = SUM('Table1'[Sales])

-- Total Orders
Total Orders = DISTINCTCOUNT('Table1'[Order ID])

-- Average Order Value
Average Order Value = DIVIDE([Total Sales], [Total Orders], 0)
```

---

## 📈 Visuals and Insights  

### 1. Total Sales by Month (Line Chart)
- Displays monthly sales trends across the year.  
- **Insight:** Sales peak in **December**, likely due to holiday demand.  
  Early months show lower sales — potential off-season period.

### 2. Total Sales by Product Name (Bar Chart)
- Shows top-selling products by revenue.  
- **Insight:** *HON 5400 Series* contributes the highest sales volume — key product for profitability.

### 3. Total Sales by Sub-Category (Tree Map)
- Breaks down sales across sub-categories under the Furniture category.  
- **Insight:** *Chairs* and *Tables* dominate, followed by *Bookcases* — focus areas for inventory and promotions.

### 4. Total Sales by Region (Pie Chart)
- Visualizes regional contribution to total sales.  
- **Insight:**  
  - **West Region (34%)** leads in total sales.  
  - **South Region (15%)** lags — could benefit from marketing push.

### 5. Average Order Value by Segment (Donut Chart)
- Compares order values by customer segment (*Consumer*, *Corporate*, *Home Office*).  
- **Insight:** All segments perform similarly, with *Corporate* and *Home Office* slightly higher — ideal targets for bulk or premium sales.

### 6. Category and Year-Month Slicers
- Provide interactivity for filtering by product category or time period.  
- **Insight:** Allows flexible exploration of performance metrics across months or product groups.

---

## ⚙️ Step-by-Step Dashboard Creation  

### 1. 🧩 Data Import  
- Imported **US Store Sales dataset** into Power BI (`Table1`).  
- Cleaned and formatted columns — ensured numeric data types for *Sales*, *Profit*, *Quantity*.  

### 2. 🔗 Data Modeling  
- Validated relationships between tables.  
- Created calculated measures using DAX (listed above).  

### 3. 🎨 Dashboard Design  
- Applied **blue gradient theme** for visual contrast.  
- Used KPI cards for top metrics: *Total Sales*, *Profit*, *Total Orders*, *AOV*.  

### 4. 📊 Visual Components  
- **Line Chart:** Total Sales by Month  
- **Bar Chart:** Total Sales by Product Name  
- **Tree Map:** Total Sales by Sub-Category  
- **Pie Chart:** Total Sales by Region  
- **Donut Chart:** Average Order Value by Segment  
- **Slicers:** Category and Year-Month  

### 5. 🧾 Formatting and Layout  
- Ensured uniform color scheme and readable font sizes.  
- Added titles, labels, legends for clarity.  
- Adjusted alignment and spacing for a clean look.  

### 6. ✅ Testing and Validation  
- Cross-checked total values and filters for accuracy.  
- Ensured slicers interact properly with all visuals.  

### 7. 💾 Export and Documentation  
- Exported dashboard view as image (`<img width="1733" height="800" alt="Screenshot 2025-10-10 183539" src="https://github.com/user-attachments/assets/1176ae39-8b7d-4258-9b3f-ae1c25640bc7" />
`).  
- Documented project details and DAX formulas in this README.  

---

## 💡 Business Insights Summary  

- **West region** drives the highest sales (34%), while **South** shows growth potential.  
- **Furniture category** performs best, especially *Chairs* and *Tables*.  
- **December** experiences the highest monthly sales — seasonal trend opportunity.  
- **Average Order Value (₹420.63)** indicates medium-ticket product dominance.  
- All customer segments contribute nearly equally — consistent demand base.  

--- 

```

---

🚀 Tools Used  
- **Power BI Desktop**  
- **Microsoft Excel / CSV Dataset**  
- **DAX for Calculated Measures**  

---

 🏁 Conclusion  
This dashboard effectively provides a **360° view of store performance**, empowering stakeholders to identify top products, strong regions, and customer segments that drive sales growth.  

---

Author: Sushmitha D  
Created Using:** Power BI  
Date:October 2025  
