# Business Insights 360

## Project Overview

AtliQ Hardware has experienced significant growth in recent years and decided to adopt data analytics using Power BI to outpace competitors and enhance decision-making. This initiative aims to address stakeholder queries across various domains such as finance, sales, marketing, and supply chain.

I worked on this project by following the Codebasics PowerBi Course, Link to the course is [here](https://codebasics.io/bootcamps/data-analytics-bootcamp-with-practical-job-assistance?utm_campaign=dataanalyticsbootcamp&utm_id=googleadspaid&gad_source=1&gclid=Cj0KCQjwztOwBhD7ARIsAPDKnkDs79RdFwkyz6S1qzIfPIK4qzgba2Pq3bfgK-eGVtLDO8a5vIDMR74aAvyUEALw_wcB)

## Technologies Used

- SQL
- PowerBi Desktop
- Excel
- DAX (Data Analysis Expressions) language
- DAX studio (for report optimizing)
- Project Charter Document

## Power BI Skills Acquired

- Identifying key questions before initiating a project
- Creating calculated columns
- Crafting measures using DAX
- Data modeling techniques
- Utilizing Bookmarks for toggling between visuals
- Implementing page navigation with buttons
- Avoiding division by zero errors using the DIVIDE function
- Creating date tables with M language
- Dynamic title generation based on filters
- Integrating KPI indicators
- Applying conditional formatting with icons or colors
- Data validation strategies
- Power BI services
- Publishing reports on Power BI services
- And much more 😅

## Key Business Concepts

- Gross price
- Pre-invoice deductions
- Post-Invoice deductions
- Net Invoice sale
- Gross Margin
- Net sales
- Net profit
- COGC - cost of goods sold
- YTD - Year to Date
- YTG - Year to Go
- Direct
- Retailer
- Distributors
- Consumer

## Company Background

AtliQ Hardware, a rapidly expanding global company, specializes in selling computers and accessories through various channels, including retail, direct sales, and distributors. The company recently faced a setback after opening stores in America based on limited data and intuition rather than comprehensive analysis. Meanwhile, competitors are leveraging extensive analytics teams for data-driven decisions. As a result, AtliQ Hardware is prioritizing the development of its own analytics team to remain competitive.


The project began with a kick-off session where objectives, expectations, and potential risks were discussed. Below are some essential questions raised before starting the dashboard development:

- Key Questions Before Starting the Dashboard
- What is the purpose of this Power BI dashboard?
- How will the success of the project be measured?
- What is the project timeline?
- Are stakeholders expecting previews before the final release?
- What outcomes do stakeholders anticipate from this project?
- What concerns do stakeholders have about the dashboard's development?
- Who will use this dashboard, and for what purposes?
- What are the stakeholders' expectations upon project completion?
- What challenges could arise during the project?
- What resources or data are needed to build the dashboard?
- Do stakeholders have any design or visual input for the dashboard?
- Following the kick-off meeting, the data engineering team provided the necessary datasets for analysis. Let’s explore them.

### Understanding the Dataset

A thorough understanding of the available data is crucial before beginning any analysis. This project involved both dimension and fact tables:

Dimension Tables: Contain static data like customer and product details.
Fact Tables: Contain transactional data.

gdb041:
dim_customer
- 27 distinct markets (e.g., India, USA, Spain)
- 75 distinct customers across markets
- 2 platform types: Brick & Mortar (physical stores) and E-commerce (online stores like Amazon, Flipkart)
- 3 sales channels: Retailer, Direct, Distributors

dim_market
- 27 distinct markets across 7 sub-zones and 4 regions: APAC, EU, NAN, LATAM

dim_product
- Product divisions: P&A (Peripherals & Accessories), PC (Notebook & Desktop), N&S (Networking & Storage)
- 14 categories (e.g., Internal HDD, Keyboard)
- Multiple variants for each product

fact_forecast_monthly
- Used for forecasting customer demand to improve satisfaction and reduce storage costs
- Denormalized for analytical purposes, with all dates in a month replaced by the start date
- Contains forecast quantities for each customer

fact_sales_monthly
- Similar to the fact_forecast_monthly table but records actual sales quantities instead of forecasts.

gdb056:
- freight_cost: Details of travel and other costs per market, categorized by fiscal year.
- gross_price: Contains product gross prices with corresponding product codes.
- manufacturing_cost: Details of manufacturing costs per product code by year.
- pre_invoice_deductions: Pre-invoice deduction percentages per customer, categorized by year.
- post_invoice_deductions: Details of post-invoice and other deductions.

## Importing Data into Power BI

- As the data is stored in a MySQL database, it was imported into Power BI using the necessary database credentials.

## Data Modeling

- Data modeling is the foundation of any report, directly impacting its performance. In this project, we used the below snowflake schema for data modeling.

<img src="https://github.com/SandeepanBhattacharyya/Business-Analytics-360-Project/blob/main/Data%20Model.png" class="center">

### Dashboard Design

Using the mockups provided, the team designed visuals and created necessary measures as the project progressed.

## Home view

The Home View provides buttons for navigating to different sections of the dashboard, including:

- Info View
<img src="https://github.com/SandeepanBhattacharyya/Business-Analytics-360-Project/blob/main/Info%20Page.png" class="center">
- Finance View
<img src="https://github.com/SandeepanBhattacharyya/Business-Analytics-360-Project/blob/main/Finance%20View.png" class="center">
- Sales View
<img src="https://github.com/SandeepanBhattacharyya/Business-Analytics-360-Project/blob/main/Sales%20View.png" class="center">
- Marketing View
<img src="https://github.com/SandeepanBhattacharyya/Business-Analytics-360-Project/blob/main/Marketing%20View.png" class="center">
- Supply chain View
<img src="https://github.com/SandeepanBhattacharyya/Business-Analytics-360-Project/blob/main/Supply%20Chain%20View.png" class="center">

Access the full report here : [Report](https://project.novypro.com/KPuDEf)


## Project Outcome

This report enables data-driven decision-making, allowing stakeholders to answer various "why" questions based on different scenarios.
