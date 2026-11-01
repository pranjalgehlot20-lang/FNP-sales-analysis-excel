FNP Sales Analysis | Excel

An end-to-end sales analysis project using Microsoft Excel to explore revenue performance, customer spending, product trends, occasion-based sales, and delivery operations for Ferns N Petals (FNP).

Tools: Microsoft Excel | Power Query | Power Pivot | PivotTables | Data Model | Excel Charts | Slicers | Timelines

⸻

1. Project Overview

Ferns N Petals (FNP) is a gifting company that delivers products for occasions such as birthdays, anniversaries, Diwali, Holi, Raksha Bandhan, and Valentine’s Day.

This project analyses FNP’s sales dataset to understand business performance across different dimensions, including revenue, products, customer orders, locations, occasions, and delivery duration.

The project follows a practical Data Analyst workflow, starting with understanding the business problem and preparing the data, followed by data modelling, analysis, visualization, and communicating actionable insights through an interactive Excel dashboard.

2. Business Problem – Why Was This Analysis Needed?

A business generates large amounts of transactional data, but raw data alone does not provide meaningful insights.

FNP needs to understand:

* Which products and categories generate the most revenue?
* How does sales performance change across different months?
* Which cities contribute the highest number of orders?
* How does customer spending vary?
* Which occasions generate higher revenue?
* Which products are popular during specific occasions?
* How long do orders take to reach customers?
* Is order quantity associated with delivery duration?

The objective was to convert the available sales data into meaningful business information that could support sales planning, product selection, promotional strategies, and operational review.

3. Project Objectives – What Did We Aim to Achieve?

1. Analyse overall sales and revenue performance.
2. Understand monthly sales fluctuations.
3. Identify high-performing products and categories.
4. Examine customer spending patterns.
5. Analyse geographical order distribution.
6. Compare revenue generated across different occasions.
7. Investigate delivery duration and its relationship with order quantity.
8. Develop an interactive dashboard for business exploration.

4. Dataset Description

The project uses three CSV datasets:

Dataset	Records	Description
Customers	100	Customer information and customer identifiers
Orders	1,000	Order details, quantities, dates, locations, and occasions
Products	70	Product names, categories, prices, and related attributes

The three datasets were connected using their respective identifiers to support analysis across customers, products, and orders.

5. Tools and Technologies

Tool	Purpose
Microsoft Excel	Main environment for data analysis and dashboard development
Power Query	Data import, inspection, cleaning, and transformation
Power Pivot	Data modelling and relationship management
Excel Data Model	Connecting multiple datasets
PivotTables	Data aggregation and business analysis
Excel Charts	Visual representation of findings
Slicers and Timelines	Interactive dashboard filtering

6. Data Preparation – How Was the Data Prepared?

Power Query was used to import and prepare the three datasets.

The following activities were performed:

* Inspected dataset dimensions, columns, data types, and data quality.
* Reviewed column distributions and profiles.
* Examined missing values and duplicate records.
* Corrected data types where required, including converting contact fields to text.
* Created additional analytical columns:
    * Month
    * Order Hour
    * Delivery Duration
    * Delivery Hour
* Merged product prices into the Orders table using Product_ID.

The prepared data was then loaded into the Excel Data Model.

7. Data Modelling

Power Pivot was used to establish relationships between the three datasets.

Relationships created:

* Customers[Customer_ID] → Orders[Customer_ID]
* Products[Product_ID] → Orders[Product_ID]

The Orders table acts as the central transactional table, connected to the Customers and Products tables.

A calculated Revenue column was created:

Revenue = Quantity × Price

This allowed revenue to be analysed across different business dimensions using PivotTables.

8. Data Analysis – How Was the Analysis Performed?

PivotTables were used to summarise and analyse the data.

The analysis covered:

* Total revenue and order count.
* Average delivery duration.
* Average revenue per order.
* Monthly revenue trends.
* Product and category performance.
* City-wise order distribution.
* Occasion-wise revenue.
* Product popularity across occasions.
* Order quantity versus delivery duration.

Correlation analysis was also performed to investigate the linear relationship between order quantity and delivery duration.

9. Business Questions and Key Findings

The project addressed the ten business questions provided in the original problem statement.

No.	Business Question	Result / Approach
1	Total Revenue	₹35,20,984
2	Average Order and Delivery Time	Average delivery duration: 5.53 days
3	Monthly Sales Performance	Analysed monthly revenue fluctuations using PivotTables
4	Top Products by Revenue	Identified the top five revenue-generating products
5	Customer Spending Analysis	Average Order Value: approximately ₹3,520.98
6	Sales Performance by Top 5 Products	Compared revenue generated by the leading five products
7	Top 10 Cities by Number of Orders	Identified the ten cities with the highest order counts
8	Order Quantity vs. Delivery Time	Correlation coefficient: approximately 0.003478
9	Revenue Comparison Between Occasions	Compared revenue across different occasions
10	Product Popularity by Occasion	Identified occasion-specific product popularity patterns

Important Analytical Findings

Overall Revenue

The business generated total revenue of ₹35,20,984 across 1,000 orders.

Average Delivery Duration

The average delivery duration was 5.53 days, providing a descriptive measure of delivery performance.

Average Order Value

Average revenue per order was approximately ₹3,520.98.

Order Quantity vs. Delivery Duration

The correlation coefficient was approximately 0.003478.

This indicates a negligible linear relationship between order quantity and delivery duration in the analysed dataset. Higher order quantities did not show a meaningful linear association with longer delivery durations.

Product Popularity by Occasion

The analysis showed that product popularity varied across occasions. Different occasions had different leading products rather than one universally popular product.

Detailed question-wise findings and interpretations are provided in FNP_Project_Findings.pdf.

10. Dashboard Development

An interactive Excel dashboard was developed to present the analysis in a consolidated and accessible format.

Key Performance Indicators

* Total Revenue
* Total Orders
* Average Delivery Time
* Average Order Value

Visualisations

The dashboard includes:

* Revenue by Occasion
* Revenue by Product Category
* Top 10 Cities by Number of Orders
* Monthly Revenue
* Top 5 Products by Revenue
* Revenue by Order Hour

Interactivity

Slicers and date timelines were added to allow users to filter the analysis dynamically.

The slicers and timelines were connected to the relevant PivotTables, and their functionality was tested to ensure that the corresponding charts updated correctly.

11. Business Implications – Why Do These Findings Matter?

The analysis provides several useful perspectives for business decision-making:

* Monthly revenue patterns can help identify periods of stronger and weaker sales activity.
* Product and category performance can support merchandising and promotional decisions.
* City-wise order distribution can help identify geographical demand concentration.
* Occasion-based revenue and product popularity can support occasion-specific marketing and product planning.
* Average delivery duration provides a baseline for reviewing delivery operations.
* Correlation analysis helps examine whether order quantity is associated with delivery duration.

These findings provide exploratory insights and should be considered alongside other business information before making operational decisions.

12. Limitations and Considerations

* The analysis is based on the available dataset and does not establish causation.
* Average Order Value represents revenue per order, not average spending per unique customer.
* A near-zero correlation does not rule out non-linear relationships or other factors affecting delivery duration.
* Monthly results should be interpreted using the correct year filter.
* Occasion-level revenue totals should be reconciled against overall revenue before being treated as a complete breakdown.

13. Project Structure

fnp-sales-analysis-excel/
│
├── Project_1.xlsx
│
├── README.md
│
├── FNP_Project_Findings.pdf
│
└── dashboard/
    └── Dashboard_Screenshot.png

14. Conclusion

This project demonstrates a practical Excel-based data analytics workflow, covering the complete process from understanding a business problem to communicating analytical findings.

By combining Power Query, Power Pivot, the Excel Data Model, PivotTables, and interactive visualisations, the project transforms raw transactional data into an interactive sales analysis dashboard.

The analysis provides insights into revenue performance, product trends, customer spending, geographical demand, occasion-based sales, and delivery operations.

The project demonstrates how Excel can be used not only for calculations and reporting, but also for structured business analysis and data-driven decision support.
