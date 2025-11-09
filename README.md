
# 🛒 Blinkit Grocery Sales & Performance Analytics Dashboard

The **Blinkit Analysis Dashboard** is a professional **business intelligence project** developed using **Microsoft Power BI** to analyze and visualize Blinkit’s grocery sales performance.  
It transforms raw transactional data into **interactive, data-driven insights** on sales trends, customer satisfaction, and outlet performance, enabling **strategic decision-making** for business growth.

---

## 📊 Project Overview

This Power BI dashboard delivers an in-depth performance view of Blinkit’s grocery operations.  
It analyzes **key business metrics**, identifies **top-performing products and outlets**, and evaluates **customer feedback trends** across multiple business dimensions.

Through advanced DAX calculations and intuitive visuals, the report supports decision-makers in optimizing:
- Product inventory and pricing
- Outlet performance and expansion
- Customer experience and satisfaction
- Regional and category-level sales strategy

---

## 🎯 Objectives

- Examine total, average, and item-level sales performance  
- Identify high-performing product categories and fat-content types  
- Assess outlet performance by **size**, **location**, and **establishment year**  
- Evaluate the relationship between customer **ratings** and **sales**  
- Deliver **data-backed recommendations** for operational improvement  

---

## 🧾 Dataset Description

**File:** `BlinkIT_Grocery_Data.xlsx`  
**Source:** Mock retail dataset modeled after Blinkit’s grocery sales operations  

| Column Name | Description |
|--------------|--------------|
| Item Identifier | Unique code for each grocery item |
| Item Type | Product category (Dairy, Snacks, Fruits, etc.) |
| Fat Content | Nutritional category (Low Fat / Regular) |
| Item Sales | Total revenue per product |
| Rating | Average customer satisfaction rating |
| Outlet Identifier | Unique outlet/store code |
| Outlet Size | Outlet classification: Small / Medium / Large |
| Outlet Location Type | Tier 1 / Tier 2 / Tier 3 city |
| Establishment Year | Year the outlet began operations |

---

## 📈 Key Performance Indicators (KPIs)

| KPI | Description |
|-----|--------------|
| 💰 **Total Sales** | Total revenue generated across all products and outlets |
| 🛍️ **Average Sales** | Mean sales per item or outlet |
| 📦 **Number of Items Sold** | Total count of distinct grocery items sold |
| ⭐ **Average Rating** | Mean customer satisfaction score |

### 📘 DAX Measures Used
```DAX
Total Sales = SUM(Data[Item_Outlet_Sales])
Average Sales = AVERAGE(Data[Item_Outlet_Sales])
Number of Items = DISTINCTCOUNT(Data[Item_Identifier])
Average Rating = AVERAGE(Data[Rating])
````

---

## 📊 Dashboard Insights

The report is structured into multiple analytical views:

1. **Overview Page**

   * Displays key KPIs: Total Sales, Average Sales, Items Sold, and Average Rating.

2. **Sales by Fat Content**

   * Compares total and average sales between low-fat and regular items.

3. **Sales by Item Type**

   * Highlights the top-selling grocery categories and their contribution to revenue.

4. **Sales by Outlet Size**

   * Visualizes revenue contribution by outlet size (Small / Medium / Large).

5. **Sales by Establishment Year**

   * Tracks performance trends over time based on outlet age.

6. **Sales by Location Type**

   * Examines how urban tier affects sales and customer ratings.

7. **Outlet Summary Metrics**

   * Provides a consolidated table of KPIs by outlet for management review.
  
     <img width="1919" height="1018" alt="Screenshot 2025-08-24 143432" src="https://github.com/user-attachments/assets/8b3b0688-e5d4-4eaa-b9ec-4efd4688be42" />


---

## 🧠 Insights & Business Findings

* **Low-fat items** generated the highest sales and customer ratings, indicating strong consumer preference for healthy options.
* **Medium-sized outlets** achieved the best revenue performance, balancing volume and customer reach.
* **Tier-1 cities** contributed the majority of sales, while **Tier-3 cities** showed growth potential.
* **Dairy and Snack categories** consistently ranked among the top-performing product types.

---

## 🛠️ Tools & Technologies

| Tool / Technology                   | Purpose                                   |
| ----------------------------------- | ----------------------------------------- |
| **Microsoft Power BI**              | Data visualization and dashboard design   |
| **Microsoft Excel**                 | Data cleaning and preprocessing           |
| **Power Query Editor**              | ETL (Extract, Transform, Load) operations |
| **DAX (Data Analysis Expressions)** | Custom KPI and measure calculations       |
| **Microsoft PowerPoint**            | Project requirement documentation         |

---

## 📂 Project Structure

```
Blinkit-Analysis/
│
├── Blinkit_Analysis.pbix             # Power BI dashboard file
├── BlinkIT_Grocery_Data.xlsx         # Dataset file
├── Blinkit_Requirements.pptx         # Requirement and design document
├── README.md                         # Project documentation
└── assets/                           # Screenshots and visuals (optional)
```

---

## ⚙️ How to Use the Dashboard

1. Install **[Power BI Desktop](https://powerbi.microsoft.com/)**.
2. Download or clone this repository:

   ```bash
   git clone https://github.com/Narendra8790/Blinkit-Grocery-Sales-Performance-Analytics.git
   ```
3. Open `Blinkit_Analysis.pbix` in Power BI Desktop.
4. Ensure `BlinkIT_Grocery_Data.xlsx` is in the same directory.
5. Click **Refresh** to load data and interact with visuals.

---

## 🚀 Future Enhancements

* Integrate **Python-based forecasting** for sales prediction
* Automate data refresh using **Power BI Service**
* Add **geospatial analysis** for outlet distribution insights
* Implement **customer segmentation (RFM analysis)** for targeted marketing

---

## 📜 License

This project is released under the **MIT License** — you are free to use and modify it for educational or portfolio purposes.

