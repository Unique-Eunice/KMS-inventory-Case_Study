# KMS_Inventory 

## Table of Contents

- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Tools and Technology](#tools-and-technology)
- [Data Cleaning and Preparation](#data-cleaning-and-preparation)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Analysis](#data-analysis)
- [Results And Findings](#results-and-findings)
- [Recommendations](#recommendations)
- [Limitations](#limitations)
- [References](#references)
  

### Project Overview
This data analysis project aims to Provide insights into the Customer order data. By analyzing various aspects of the Order data, we wish to identify trends, make data-driven Recommendations and gain a stronger understanding of the Company's Performance.

### Data Sources

Kultra Mega Stores: The primary dataset used for this analysis is the dataset scaraped from "KMS Inventory" containing detailed information about Order Data from 2009-2012.

### Tools and Technology

- Microsoft Excel- Data cleaning, Pivot Tables, Dashboard [Download_here](https//microsoft.com)
- Microsoft SQL Server [Download_here](https//microsoft.com) 
- Git & GitHub for version control.

### Data Cleaning and Preparation

In the initial data preparation phase, we performed the following tasks:
1. Data loading and inspection.
2. Handling missing values and duplicate.
3. Clean complex product category hierarchies for easier analysis.
4. Simplify product names for better reporting.
5. Data cleaning and formating.

### Exploratory Data Analysis
EDA involvoed exploring the Product and Review data to answer key questions, such as:
1. Which product category had the highest sales?
2. What are the Top 3 and Bottom 3 regions in terms of sales?
3. What were the total sales of appliances in Ontario?
4. Advise the management of KMS on what to do to increase the revenue from the bottom
10 customers
5. KMS incurred the most shipping cost using which shipping method?
6. Who are the most valuable customers, and what products or services do they typically
purchase?
7. Which small business customer had the highest sales?
8. Which Corporate Customer placed the most number of orders in 2009 – 2012?
9. Which consumer customer was the most proftable one?
10. Which customer returned items, and what segment do they belong to?
11. If the delivery truck is the most economical but the slowest shipping method and
Express Air is the fastest but the most expensive one, do you think the company
appropriately spent shipping costs based on the Order Priority
### Data Analysis

``` SQL
Select * From KMS Inventory

SELECT *
FROM KMS Inventory
WHERE Order_ID IS NULL
   OR Product_Name IS NULL
   OR Customer_Name IS NULL
   OR Sales IS NULL;
```

### Results And Findings

The analysis results are summarized as follows:

- Technology generated the highest total sales (₦5,984,248.50).
- Top 3 Regions: West, Ontario, Prarie.
- Bottom 3 Regions: Yukon, Northwest Territories, Nunavut.
- Total sales of appliances in Ontario amounted to approximately ₦202,346.84, showing opportunity for targeted growth.
- Delivery Truck incurred the highest total shipping cost (₦52,016).
- The customers with the highest overall sales predominantly purchased Technology and Office Supplies products.
- A specific Small Business customer (details obtainable from SQL) had the highest sales within this segment.
- One Corporate customer placed the most orders during this period, highlighting high engagement.
- Some customers returned items, identifiable through negative sales/profit figures. These customers belong to mixed segments, suggesting returns are not isolated to one group.

### Recommendations

- **Capitalize on the success of Technology by introducing complementary products, bundling offers, or targeted promotions.
- **Yukon, Northwest Territories, and Nunavut require strategic marketing, distribution improvements, or pricing incentives to boost sales.
- **Ontario shows promising appliance sales; targeted promotions, seasonal discounts, or local partnerships could drive further revenue.
- **Conduct an audit to ensure high-priority orders use Express Air despite higher cost for speed and Low-priority orders leverage Delivery Truck for cost-efficiency.
- **Provide bulk order discounts or loyalty incentives to retain high-order Corporate clients, especially those active between 2009–2012.

### Limitations

I had to replace some missing values with assumed values and i also had to remove some data that would have affected the accuracy of my analysis.

### References
1. Incubator hub
2. Her Data Project
3. Data Camp
4. Chatgpt
   





