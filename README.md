# Power BI Sales Dashboard Project

## Objective of the Sales Dashboard / Business Problem

The objective of this report is to analyze and present comprehensive insights into sales, profit, orders, profit margin, and various comparisons. Using Power BI, this dashboard provides a clear understanding of key performance indicators and trends.

### Report Objectives:
1. **Calculate Total Sales:** Display the total sales value for the selected period to understand overall revenue.
2. **Calculate Profit:** Visualize the total profit achieved based on sales data.
3. **Analyze Orders:** Examine the number of orders placed during the selected period.
4. **Calculate Profit Margin:** Assess the profitability of products or services.
5. **Compare Sales by Product with Previous Year:** Highlight growth or decline in product sales.
6. **Compare Sales by Months with Previous Year:** Identify trends in sales performance across months.
7. **Display Top 5 Cities:** Showcase cities generating the highest sales.
8. **Compare Profit by Channel with Previous Year:** Understand profitability across different channels.
9. **Analyze Sales by Customer:** Highlight performance of individual customers and compare year-over-year.
10. **Create Slicers:** Enable dynamic filtering by date, city, product, and channel.

---

## Steps to Follow for an End-to-End Power BI Project

### 1. Gather Data
- Collect necessary data from sources such as databases, spreadsheets, or web services.
- Ensure data accuracy and relevance to the objectives.

### 2. Power Query – Data Extract, Transform & Load (ETL)
- Use Power Query Editor to clean and transform data:
  - Remove duplicates.
  - Handle missing values.
  - Merge datasets or create calculated columns.

### 3. Create a Date Table
- Use a date table for DAX time intelligence functions.
- Disable Auto Date/Time in Power BI Options for better performance.

### 4. Create Data Model in Power BI Desktop
- Design relationships between tables and establish hierarchies.
- Ensure accurate modeling for reliable analysis and visualizations.

### 5. Develop Reports in Power BI Desktop
- Create visualizations such as:
  - **Sales by Product** (with year-over-year comparison).
  - **Sales by Month** (with year-over-year comparison).
  - **Top 5 Cities by Sales**.
  - **Profit by Channel** (year-over-year comparison).
  - **Sales by Customer** (year-over-year comparison).
- Include cards for:
  - Total Sales
  - Profit
  - Profit Margin
  - Products Sold

### 6. Implement DAX Calculations
- Use DAX for measures, calculated columns, and complex aggregations:
  - **Total Sales:** `Sales = SUM(Sales_Data[Sales])`
  - **Previous Year Sales:** `Sales PY = CALCULATE([Sales], SAMEPERIODLASTYEAR(DateTable[Date]))`
  - **Difference Between Current and Previous Year Sales:** `Sales vs PY = [Sales] - [Sales PY]`
  - **Year-over-Year Percentage Change:** `Sales vs py % = DIVIDE([Sales vs PY], [Sales], 0)`
  - **Profit Margin:** `Profit Margin = DIVIDE([Profit], [Sales], 0)`

---

## Conclusion of Power BI Sales Dashboard Project

### Key Findings for the Year 2019:
- **Sales:** Decreased by over 10%.
- **Top Products:** Sales dropped for the top 7 products.
- **Customer Impact:** Four customers significantly contributed to the sales decline.
- **Profit Margin:** Higher in the export channel.

### Additional Insights:
Further insights can be derived based on the detailed analysis and visualizations provided.

---

## Features of the Dashboard:
- Interactive slicers for dynamic filtering.
- Year-over-year comparisons for sales and profit.
- Focused visualizations on top-performing cities, channels, and customers.
