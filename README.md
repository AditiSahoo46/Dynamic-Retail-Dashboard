# Dynamic-Retail-Dashboard
## Overview

The **Dynamic Retail Dashboard** is an interactive, data-driven Excel solution designed to analyze and visualize retail performance. The dashboard integrates datasets hosted on GitHub, leverages **Power Query** for data transformation, and uses **Pivot Tables, charts, slicers, and KPIs** to deliver actionable business insights.

This dashboard enables stakeholders to monitor performance, identify trends, and make informed, data-driven decisions.

---

## Datasets Used

### 1. Orders Table

Contains transactional details related to customer orders, including product, shipping, sales, and profitability metrics.

**Key Fields:**

* Order ID
* Returned
* Order Date & Ship Date
* Ship Mode
* Customer Name & Segment
* Country & Market
* Sales, Profit, Discount

<img width="757" height="153" alt="image" src="https://github.com/user-attachments/assets/366d5308-e679-414b-8aa3-b0840c1b237d" />


**Sample Data:**

| Order ID       | Returned | Order Date | Ship Mode    | Segment   | Country       | Market | Sales   | Profit  | Discount |
| -------------- | -------- | ---------- | ------------ | --------- | ------------- | ------ | ------- | ------- | -------- |
| CA-2012-124891 | No       | 31-07-2020 | Same Day     | Consumer  | United States | US     | 2309.65 | 762.18  | 0        |
| IN-2013-77878  | Yes      | 05-02-2021 | Second Class | Corporate | Australia     | APAC   | 3709.40 | -288.77 | 0.1      |

---

### 2. Returns Table

Tracks returned orders and their associated markets.

**Key Fields:**

* Order ID
* Returned
* Market

---

### 3. People Table

Contains sales representatives and their assigned regions.

**Key Fields:**

* Person
* Region

---

## Business Problems Solved & Implementation Steps

### 1. Key Performance Indicators (KPIs)

**Objective:**
Display critical business metrics dynamically.

**KPIs Included:**

* Total Sales
* Total Profit
* Total Quantity
* Number of Orders
* Profit Margin

**Steps:**

* Imported Orders data using Power Query
* Created calculated columns (Profit Margin = Profit / Sales)
* Used Excel formulas:

  * Total Sales: `SUM(Sales)`
  * Total Profit: `SUM(Profit)`
  * Total Quantity: `SUM(Quantity)`
  * Number of Orders: `COUNT(Order ID)`
* Designed a dynamic KPI section with icons and conditional formatting

---

### 2. Sales & Profit Trend Analysis

**Objective:**
Identify trends and seasonality in sales and profit.

**Steps:**

* Created Pivot Table grouped by Year and Month (Order Date)
* Added Sales and Profit as values
* Visualized trends using Line Charts
* Enabled dynamic filtering with slicers (Market, Region, Category)

<img width="355" height="333" alt="image" src="https://github.com/user-attachments/assets/9213abd1-3491-4206-af53-c0ce5b9d90b6" />


---

### 3. Category-Wise Profit Analysis

**Objective:**
Evaluate profitability across product categories.

**Steps:**

* Pivot Table with Category as rows and Profit as values
* Sorted categories by descending profit
* Visualized results using a Bar Chart
* Added slicers for interactive analysis

<img width="362" height="332" alt="image" src="https://github.com/user-attachments/assets/d63022e7-e0cb-49e9-a701-b1b46be046cb" />

---

### 4. Segment-Wise Sales Share (%)

**Objective:**
Analyze contribution of each customer segment to total sales.

**Steps:**

* Pivot Table with Segment and Sales
* Calculated percentage contribution
* Used Pie/Donut Chart to display sales share
* Enabled dynamic labels and slicers

<img width="351" height="329" alt="image" src="https://github.com/user-attachments/assets/4ef8a797-c0f6-4754-a544-f4b65d5ab695" />


---

### 5. Sales by Country

**Objective:**
Identify top-performing countries.

**Steps:**

* Pivot Table with Country and Sales
* Sorted countries by sales volume
* Applied conditional formatting / heatmap to highlight performance

<img width="342" height="336" alt="image" src="https://github.com/user-attachments/assets/40a75496-6d0b-425e-a87b-f07b7a54fa80" />


---

### 6. Top 5 Sub-Categories

**Objective:**
Identify the best-performing sub-categories.

**Steps:**

* Pivot Table with Sub-Category and Sales
* Sorted by Sales (descending)
* Filtered Top 5 Sub-Categories
* Visualized using a Column Chart

<img width="352" height="336" alt="image" src="https://github.com/user-attachments/assets/2c12105b-6556-4a5a-b126-4663d341ee9a" />


---

### 7. Bottom 5 Subcategories

**Objective:**
Highlight the bottom 5 subcategories with the lowest sales performance.

**Steps:**

1. Use the existing Pivot Table with **Sub-Category** in rows and **Sales** as values.
2. Sort the Pivot Table by **Sales in ascending order** to bring the lowest sales to the top.
3. Apply a **Value Filter** to show only the **Bottom 5** subcategories by sales.
4. Create a **Column Chart** based on the filtered data.
5. Use contrasting colors (e.g., red or orange) in the chart to emphasize the low-performing subcategories clearly.

<img width="294" height="270" alt="image" src="https://github.com/user-attachments/assets/a06668b7-81bd-45c6-941b-e7701320a03a" />

---


## Dynamic Features

* **Interactive Slicers** for real-time filtering
* **Dynamic Charts** that update instantly based on selections
* **Power Query Automation** for data cleaning and refresh
* **Central KPI Panel** for quick performance monitoring

---

## Future Enhancements

* Return Rate Analysis by Market & Category
* Top & Bottom Customers by Profitability
* Market-Level Performance Comparison
* Product-Level Contribution Analysis

---

## Business Impact

This dashboard helps retail organizations:

* Monitor performance using KPIs
* Understand trends across categories, segments, and geographies
* Identify growth opportunities and operational inefficiencies
* Support data-driven strategic decisions

---

## Visuals

The repository includes:

* Visual examples for each analysis
* Screenshots of the final interactive dashboard

<img width="810" height="569" alt="image" src="https://github.com/user-attachments/assets/41510bd2-1039-4d75-8989-28bdd7eeec80" />


---

