# Coffee-Sales-Dashboard---Excel-Project
This project is an end-to-end Excel-based analysis of coffee sales data sourced from Kaggle. It involves data cleaning, transformation, and visualization using pivot tables, charts, and interactive dashboard elements. The final dashboard lets users explore sales trends, top customers, and country-wise performance with filters and slicers.

## 📌 Project Overview

This project focuses on analyzing coffee sales data and creating an interactive Excel dashboard to visualize key insights. The dataset is sourced from Kaggle and has been cleaned, transformed, and structured using Excel formulas and pivot tables.

## 🎯 Objectives

- Transform raw sales data into meaningful insights.
- Use Excel's advanced features to create an interactive dashboard.
- Provide a clear visual representation of sales trends, top customers, and country-wise performance.

## 🔧 Tech Stack

- **Microsoft Excel** (Pivot Tables, Charts, Slicers, Timelines, Formulas)
- **Data Cleaning & Transformation** (XLOOKUP, INDEX-MATCH, IF formulas)
- **Visualization** (Line Charts, Bar Charts, Slicers, Timelines)

## 📊 Dashboard Features

### **Visuals:**

- **Line Chart:** Sales trends over time for different coffee types (Arabica, Excelsa, Liberica, Robusta).
- **Bar Charts:**
  - Sales by country (U.S., Ireland, UK)
  - Top 5 customers by revenue

### **Interactivity:**

- **Timeline:** Filter sales by date.
- **Slicers:**
  - Roast Type (Dark, Light, Medium)
  - Size (0.2 kg, 0.5 kg, 1 kg, 2.5 kg)
  - Loyalty Card Status (Yes/No)

## 📂 Data Structure

The dataset consists of three key tables:

1. **Orders Table:** Order ID, Order Date, Customer ID, Product ID, Quantity, etc.
2. **Customers Table:** Customer ID, Name, Email, Country, Loyalty Card Status.
3. **Products Table:** Product ID, Coffee Type, Roast Type, Size, Unit Price, Profit.

## 🛠️ Excel Techniques Used

### **Data Gathering & Transformation:**

- **XLOOKUP** to fetch customer details based on Customer ID.
- **INDEX-MATCH** for retrieving product details.
- **IF formulas** to categorize coffee types.

### **Examples of Formulas Used:**

#### XLOOKUP Example:

```excel
=XLOOKUP(C2, Customers!A:A, Customers!B:B, "", 0)
```

#### INDEX-MATCH Example:

```excel
=INDEX(Products!A1:D100, MATCH(D2, Products!A:A, 0), MATCH(I$1, Products!1:1, 0))
```

#### Sales Calculation:

```excel
=Unit_Price * Quantity
```

#### Coffee Type Classification:

```excel
=IF(I2="ROB", "Robusta", IF(I2="EXE", "Excelsa", IF(I2="ARA", "Arabica", IF(I2="LIB", "Liberica", ""))))
```

## 📈 Creating Pivot Tables & Charts

- **Pivot Table:** Organized sales data by date and category.
- **Pivot Charts:** Used to visualize sales trends and customer insights.
- **Slicers & Timelines:** Enabled interactive data filtering.

## 🎨 Dashboard Formatting & Final Touches

- Applied **consistent styling** (colors, fonts, layout adjustments).
- Removed **gridlines** for a cleaner appearance.
- Added **scroll bars** for easy navigation.

## 🚀 Future Enhancements

- Integrating **Power BI** for more advanced analytics.
- Adding **forecasting models** to predict future sales.
- Automating data updates using **Power Query**.

---

### 🔗 Connect & Feedback

If you have any suggestions or improvements, feel free to open an issue or fork the repository!

📬 Reach out via [GitHub](https://github.com/yourusername) 🚀

