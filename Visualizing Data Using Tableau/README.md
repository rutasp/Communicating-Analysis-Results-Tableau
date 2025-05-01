# Interactive Dashboard with Tableau

This project is part of the Data Analytics course at Turing College. The goal is to create a dynamic and user-friendly sales dashboard using Tableau Public, based on the AdventureWorks company dataset. The focus is on building a dashboard that provides business-relevant insights and supports decision-making for the Sales department.

## Tools Used

- **Tableau Public**
- **Google Sheets** (as data source)
- **SQL** (for optional data extraction and preparation from BigQuery)

## Tasks Overview

### 1. Dashboard Foundations

1.1 Connect to the AdventureWorks Sales Order Data (Google Sheets)  
1.2 Add key KPIs to the top of the dashboard:
- Order Count  
- Total Sales ($)  
- Average Order Value (AOV)  
- Average Days to Ship (custom calc.)

1.3 Create two time-series charts:
- Monthly Sales by Year-Month  
- Year-over-Year Monthly Sales

1.4 Add a date range filter to the dashboard

### 2. Sales Type Breakdown

2.1 Define a calculated field `Sales Type`:  
- Online sales: `SalespersonID` is NULL  
- Offline sales: `SalespersonID` is NOT NULL  

2.2 Create a bar or area chart comparing Offline vs Online sales

### 3. Sales Reason Dynamics

3.1 Join `salesorderheader` with `salesreason`  
3.2 Account for multiple sales reasons per order  
3.3 Create a 100% stacked area chart showing distribution of reasons over time

### 4. Salesperson Performance

4.1 Create a bar chart: Total Sales per Salesperson  
4.2 Add cumulative percentage line (Table Calculation: Running Total % of Total Sales)  
4.3 Use existing dataset; no new data source needed

### 5. Geographic Analysis

5.1 Join with `salesterritory` table to map regions  
5.2 Create a Map Chart showing Total Sales by region

## Final Dashboard Enhancements

- Adjust colors to match company branding (avoid dark blue, ensure accessibility for color blindness)  
- Improve chart labeling, layout clarity, and formatting consistency  
- Add at least one new insight/KPI, e.g.:
  - Year-over-Year Growth %  
  - Average Profit Per Customer  
  - Refined Pareto Analysis  
- Use at least one parameter-based custom filter for interactivity  
- Clearly structure visuals to prioritize executive-level information at the top  
- Ensure the dashboard is self-explanatory and easy to explore

## Bonus: Analytical Considerations

- Document any additional SQL queries used to prepare data  
- Reflect on limitations of the analysis and suggest further improvements  
- Prepare for questions on Tableau best practices, including:
  - How to join data sources  
  - Effective dashboard layouts  
  - Use of preattentive attributes  
  - When a static dashboard might be more appropriate  
