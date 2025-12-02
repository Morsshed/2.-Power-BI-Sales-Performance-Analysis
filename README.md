# 2. Power-BI-Sales-Performance-Analysis
Yearly Sales Performance Analysis
 
[View the Power BI Dashboard](https://app.powerbi.com/view?r=eyJrIjoiZDM1YTRjZjEtOGZhYy00OGE2LWE3ZGItZWU0MTc0MDFlN2YxIiwidCI6IjFhOTM4M2ZmLTVlMDEtNDkzYy04MTJmLTg0ODAzZTliMGI3YiJ9)

 ### 1. Domain: Delivery

# Analysis Details
 ## i. Business Case
 
🚩 Problem Statement:

The E-Commerce Sales Analytics Dashboard aims to address several key business challenges related to sales performance, customer behavior, product profitability, and regional growth. Despite generating strong revenue and profit, the organization faces gaps in customer retention, uneven regional performance, and product return issues that impact overall business efficiency. To support data-driven decision-making, the project focuses on identifying underlying issues and converting raw transactional data into meaningful insights.

The primary business problems addressed in this project include:

✔️ Declining revenue per customer at the start of each month, indicating potential behavioral or promotional timing gaps.

✔️ High return rates in specific product categories, especially Shorts, which negatively impact profit margins and customer satisfaction.

✔️ Regional sales imbalance, with North America outperforming other regions, highlighting untapped market potential in Europe, Asia-Pacific, and South America.

✔️ Dependence on a small group of high-performing products, increasing risk if demand shifts.

✔️ Suboptimal customer retention, where many customers fall into “Potential Loyalists” or “At-Risk” segments instead of moving into loyal or champion categories.

✔️ Insufficient demographic targeting, as the business lacks actionable insights into how age, gender, and marital status influence purchase behavior.

✔️ Inefficient forecasting and inventory allocation, causing fluctuations in demand planning.

This project provides a structured analytical approach to uncover these issues and enables the business to make informed decisions regarding pricing, product strategy, customer engagement, and market expansion.

 ## ii. Snapshots
![Pizza Sales Performance Analysis](https://github.com/Morsshed/2.-Power-BI-Sales-Performance-Analysis/blob/main/Pizza%20Sales%20Performance%20Analysis.jpeg?raw=true)


 ## iii. Dashboard Features

                             Dynamic Features:
                                              1. Slicers : Pizza Category/Name/Size
                                              2. Button : Pizza Sales Part 1&2
                                              3. Nevigators : Pizza Sales Part 1                  
                             Analytical Features:
                                              1. KPI Cards : Total Orders, Total Revenue, Total Orders, Total Pizza Sold, AVG Order Value, AVG Pizzas Per Order
                                              2. Column Chart : Daily Trends of Orders,
                                              3. Line Chart : Monthly Trends of Orders
                                              4. Funnel Chart : Total Pizzas Sold by Pizza Category
                                              7. Pie Charts : % of Sales by Pizza Category, % of Sales by Pizza Size
                                              8. Bar Charts : Top & Bottom 5 Pizzas by Total Revenue/Total Quantity/Total Order
                                              
 ## iv. Insights and Recommendation

                 Summary Insights
                        1. The business has achieved 25K total orders within the selected period.
                        2. Total revenue is 25M, showing strong overall sales performance.
                        3. Net profit is 10M, resulting in an excellent 42% profit margin.
                        4. The return rate is 2.2%, indicating efficient operations and product quality.
                        5. The forecasting chart shows a clear upward trend, meaning revenue is expected to grow steadily.
                        6. “Tires and Tubes” is the most ordered product sub-category.
                        7. “Shorts” is the sub-category with the highest return rate.
                        8. “Bib-Shorts” is the top-performing product in terms of revenue and net profit.
                        9. The top 10 products by profit show that cycling gear dominates the highest revenue list.
                       10. There are 18,148 total customers, and 17,416 have made purchases, giving a strong customer purchase rate.
                       11. The average revenue per customer is approximately $1,430.
                       12. Gender distribution is nearly balanced, with slightly more male customers.
                       13. Most customers fall within the 25–34 age group, indicating a young target audience.
                       14. The customer segmentation (RFM) shows a large portion in the “Potential Loyalists” and “Champions” categories.
                       15. Revenue per customer has a declining trend at the start of the month but stabilizes later.
                       16. Single customers represent the majority of buyers, which may influence product preferences.
                       17. North America generates the highest total revenue and profit, with 42.5% profit margin.
                       18. Europe, although significant in sales volume, shows slightly lower return rates compared to NA.
                       19. Revenue is widely diversified across continents, reducing business risk.
                       20. The United States leads all countries in both revenue and total orders, followed by the U.K. and Germany.

                Recommendations for Business Growth
                       1. Focus Marketing on High-Performing Segments. It is recommended to target promotions to “Champions” and “Potential Loyalists” to maximize repeat purchases.
                       2. Improve Product Quality for High-Return Categories. It is necessary to investigate Shorts category (highest return rate) for sizing, material, or expectation mismatch issues.
                       3. Expand Inventory & Promotions for High-Demand Products. The company can increase advertising and stock for Tires and Tubes, Bib-Shorts, and other top-profit items.
                       4. Grow Underperforming Regions With High Potential. Europe and Asia-Pacific show significant order volume—launch region-specific campaigns and pricing adjustments.
                       5. Enhance Customer Lifetime Value. The company can introduce loyalty programs for young customers (25–34 age group), who represent the highest engagement segment.
 ## v. Data Source
 [Adventure Works Dataset (Kaggle)](https://www.kaggle.com/datasets/atulmittal199174/adventure-works-dataset)
# A - Analysis Techniques:
# A1 - Data Preparation (ETL & Normalization)

### Data Cleaning

✓ Removed duplicate rows and unnecessary fields to streamline the dataset.

✓ Standardized column names, formats, and units for consistency across all tables.

✓ Converted text-based date fields into proper Date formats to support time-intelligence calculations.

✓ Handled missing values using appropriate strategies (imputation or exclusion).

### Data Transformation

✓ Created new calculated columns such as Order Line Item, Retail Price, and Return Quantity to enrich analytical capabilities.

✓ Split and transformed fields where necessary to improve clarity and usability.

✓ Reassigned data types (Whole Number, Decimal, Text, Date) to ensure accurate aggregations and relationships.

✓ Applied conditional transformations to derive customer segments, product groupings, and territory regions.
