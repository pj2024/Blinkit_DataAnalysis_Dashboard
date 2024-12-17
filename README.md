# Blinkit_DataAnalysis_Dashboard
![Screenshot 2024-12-17 151518](https://github.com/user-attachments/assets/523834db-eb46-451b-8ffc-f3b38961c9ba)
# Blinkit Analysis Power BI Project  

## Overview  
The Blinkit Analysis Power BI project aims to analyze sales performance, customer satisfaction, and inventory distribution. This project provides actionable insights using interactive dashboards and various KPIs. By visualizing trends across product types, outlet sizes, locations, and customer ratings, the project enables data-driven decision-making.  

---

## Business Requirement  
To conduct a comprehensive analysis of Blinkit's sales performance, customer satisfaction, and inventory distribution to identify key insights and opportunities for optimization using various KPIs and visualizations in Power BI.  

### **KPI Requirements**  
1. **Total Sales**: Overall revenue generated from all items sold.  
2. **Average Sales**: Average revenue per sale.  
3. **Number of Items Sold**: Total count of items sold.  
4. **Average Rating**: Mean customer rating for items sold.  

---

## Steps in the Project  

### **1. Requirement Gathering**  
- Identified the need for an interactive Power BI dashboard to analyze sales, customer behavior, and inventory trends.  
- Defined KPIs and specific objectives, including Total Sales, Average Sales, Number of Items Sold, and Average Rating.  

### **2. Data Walkthrough**  
- Reviewed dataset structure and scope, including fields like sales, product attributes, outlet details, and customer feedback.  
- Identified inconsistencies like missing data and outliers.  

### **3. Data Connection**  
- Imported data from sources such as CSV files and databases into Power BI.  
- Validated data completeness and linked related tables for seamless analysis.  

### **4. Data Cleaning/Quality Check**  
- Addressed missing values in customer ratings.  
- Standardized data formats and removed duplicates.  

### **5. Data Modeling**  
- Created a star schema with:  
  - **Fact Table**: Sales data.  
  - **Dimension Tables**: Product, Outlet, and Feedback data.  
- Established relationships for efficient navigation.  

### **6. Data Processing**  
- Transformed data to create calculated fields for Total Sales, Average Sales, and other KPIs.  

### **7. DAX Calculations**  
Used DAX to implement KPI calculations:  
- **Total Sales**: `SUM(Sales[Revenue])`  
- **Average Sales**: `DIVIDE(SUM(Sales[Revenue]), COUNT(Sales[Order ID]))`  
- **Number of Items Sold**: `SUM(Sales[Quantity])`  
- **Average Rating**: `AVERAGE(Feedback[Rating])`  

### **8. Dashboard Layouting**  
- Designed the dashboard to provide clear and interactive sections:  
  1. **Sales Overview**  
  2. **Customer Satisfaction**  
  3. **Product Analysis**  
  4. **Inventory Distribution**  

### **9. Charts Development and Formatting**  
Customized visualizations to meet analysis goals:  
1. **Total Sales by Fat Content**: Donut Chart.  
2. **Total Sales by Item Type**: Bar Chart.  
3. **Fat Content by Outlet for Total Sales**: Stacked Column Chart.  
4. **Total Sales by Outlet Establishment**: Line Chart.  
5. **Sales by Outlet Size**: Donut/Pie Chart.  
6. **Sales by Outlet Location**: Funnel Map.  
7. **All Metrics by Outlet Type**: Matrix Card.  

### **10. Dashboard/Report Development**  
- Integrated all visuals into an interactive dashboard.  
- Slicers and drill-through functionality are enabled for enhanced analysis.  

### **11. Insights Generation**  
Key findings:  
- Medium-fat products generated the highest revenue.  
- Snacks and dairy were the top-performing item types.  
- Larger outlets contributed significantly to sales.  
- Certain urban locations outperformed rural areas in revenue.  

---

## Chart Details  

### 1. **Total Sales by Fat Content**  
- **Objective**: Analyze the impact of fat content on Total Sales.  
- **Chart Type**: Donut Chart.  

### 2. **Total Sales by Item Type**  
- **Objective**: Identify performance of item types.  
- **Chart Type**: Bar Chart.  

### 3. **Fat Content by Outlet for Total Sales**  
- **Objective**: Compare Total Sales across outlets segmented by fat content.  
- **Chart Type**: Stacked Column Chart.  

### 4. **Total Sales by Outlet Establishment**  
- **Objective**: Evaluate how outlet age/type influences Total Sales.  
- **Chart Type**: Line Chart.  

### 5. **Sales by Outlet Size**  
- **Objective**: Analyze the correlation between outlet size and sales.  
- **Chart Type**: Donut/Pie Chart.  

### 6. **Sales by Outlet Location**  
- **Objective**: Assess sales distribution across locations.  
- **Chart Type**: Funnel Map.  

### 7. **All Metrics by Outlet Type**  
- **Objective**: Provide a comprehensive view of all metrics by outlet type.  
- **Chart Type**: Matrix Card.  

---

## Outcome  
The Power BI dashboard provided a comprehensive analysis of Blinkit's sales and customer satisfaction metrics.  
### Benefits:  
- Identified high-performing products, regions, and outlets.  
- Highlighted trends for inventory optimization.  
- Enabled stakeholders to make data-driven decisions for sales and marketing strategies.  

---

## Technologies Used  
- **Tools**: Power BI  
- **Language**: DAX  

---

## Folder Structure  
```plaintext
|-- https://github.com/pj2024/Blinkit_DataAnalysis_Dashboard/blob/main/Blinkit%20power%20bi/BlinkIT%20Grocery%20Data.xlsx                # Raw and cleaned datasets  
|-- visuals/              # Screenshots of Power BI dashboard  
|-- README.md             # Project documentation  
|-- blinkit.pbix          # Power BI report file  
|-- insights/             # Generated insights and reports  
