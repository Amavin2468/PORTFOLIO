## Blacktech Pizza Sales Analysis

## Table of Contents

- [Project Overview](#project-overview)
- [Data Source](#data-source)
- [Tools](#tools)
- [Data Cleaning](#data-cleaning)
- [Data Modeling](#data-modeling)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Findings](#findings)
- [Recommendations](#recommendations)

### Project Overview

Pizza Sales KPI, Playing the role of a BI Consultant hired by BlackTECH's Pizza, a Canadian-inspired pizza place in Ontario. My team and I been hired to help the restaurant use data to improve operations, Sales, Products and Revenue.

### Data Source

Dataset contains 4 tables in CSV format:
- The Orders table containing the date & time that all table orders were placed
- The Order Details table contains the different pizzas served with each order in the Orders table, and their quantities
- Pizzas table contains the size and price for each distinct pizza in the Order Details table, as well as its broader pizza type
- Pizza Types table contains details on the pizza types in the Pizzas table, including their name as it appears on the menu, the category it falls under, and its list of ingredients

### Tools

- Excel - Data Cleaning
  - [Download here](https://microsoft.com)
- PowerBi - Data Modeling and Visualization
  - [Download here](https://microsoft.com)

### Data Cleaning

In the Data preparation phase, We performed the following Tasks:
1. Data Loading and inspection
2. Data cleaning and formating

### Data Modeling

1. Created relationships between the different tables, these relationships determine how the data in one table is connected to data in another.
2. Creating calculated measures using the following DAX formulas:
 - Average Sales = AVERAGEX(order_details,[Total Sales])
 - Total Sales = SUMX(order_details,order_details[quantity]*RELATED(pizzas[price]))
 - Total_Orders = COUNT([quantity])

### Exploratory Data Analysis

- What is the Overall sales trend?
- What is the Overall order trend?
- What are the peak periods?
- Which Products are top sellers?

### Findings
The analysis results are summarized as follows:
1. There is a noticeable peak on fridays and in july (summer)
2. The classic pizza is the highest selling category why the lowest selling category is the veggie

### Recommendations
1. Adjustment staffing levels based on fluctuating demand throughout the week and day to help ensure adequate coverage during peak hours while avoiding overstaffing during slower periods
2. Enhance the low-selling pizza's recipe to improve taste and appeal
3. Invest in marketing and promotions during peak sales seasons to maximize revenue

