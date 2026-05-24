# Amazon Sales Dashboard – Power BI

## Overview
This project presents an interactive **Amazon Sales Dashboard** built in **Power BI** to analyze sales performance, customer reviews, shipment distribution, and product category insights.

The dashboard provides a clean and structured visualization of:
- Total Sales
- Total Reviews
- Average Product Price
- Monthly Sales Trends
- Category-wise Sales & Reviews
- Shipment-based filtering

---

## Dashboard Preview

![Amazon Sales Dashboard](https://github.com/akisavujel/Power-BI/blob/e34cccda6bdde9534ff815bbd26f5a4fb29ef0c3/Amazon-Sales/Amazon-Dashboard.jpg)

---

## Data Cleaning & Transformation

The following preprocessing steps were completed in **Power Query Editor**:

### 1. Data Type Validation
- Verified and corrected data types for all columns.

### 2. Handling Null Values
- Replaced `null` values in the **Review** column with `3`.

### 3. Shipment Column Standardization
Fixed inconsistent shipment values:
- `IND` → `India`
- `NEP` → `Nepal`
- `United States’` → `USA`

### 4. Date Extraction
From the `order_date` column:
- Extracted **Year**
- Extracted **Month**

### 5. Validation of New Columns
- Confirmed proper data types for newly created Year and Month columns.

---

## DAX Measures Used

### Total Sales
```DAX
Total Sales = SUM(Amazon_Sales[Sales])
```

### Total Reviews
```DAX
Total Reviews = SUM(Amazon_Sales[Review])
```

### Average Product Price
```DAX
Average Product Price = AVERAGE(Amazon_Sales[Price])
```

---

## Visualizations Included

### KPI Cards
- Total Sales
- Total Reviews
- Average Product Price

### Charts
- Bar Chart → Total Sales by Product Category
- Donut Chart → Total Reviews by Product Category
- Pie Chart → Product Category Distribution
- Line Chart → Total Sales by Month

### Table Visual
Displays:
- Product Category
- Total Sales
- Total Reviews

### Slicer
- Shipment Category Filter

---

## Tools & Technologies
- Power BI Desktop
- Power Query
- DAX

---

## Key Insights
- Cameras generated the highest sales among all categories.
- Sales peaked during specific months, showing seasonal trends.
- Shipment filtering enables region-based sales analysis.
- Product review distribution highlights customer engagement across categories.

---

## Project Structure
```bash
Amazon-Sales/
│── Amazon-Dashboard.jpg
│── Amazon-Sales.pbix
│── README.md
```


