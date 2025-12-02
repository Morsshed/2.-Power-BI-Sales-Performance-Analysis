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
                                              
 ## iv. 🔍 Insights and Recommendations
 
  #### Overall Performance

       ✓ Total revenue reached $815,306, driven by consistent customer demand.

       ✓ 21,350 orders were recorded, reflecting strong customer activity.

       ✓ A total of 49,574 pizzas were sold.

       ✓ Average order value = $38.19, showing purchases often include multiple items.

       ✓ Average pizzas per order = 2.32, indicating bundling behavior.

  #### Daily & Monthly Trends

       ✓ Fridays and Saturdays generate the highest orders (weekend peaks).

       ✓ Tuesdays and Wednesdays are the slowest sales days.

       ✓ July records the highest monthly orders.

       ✓ October shows the lowest activity.

  #### Category Insights

       ✓ Classic pizzas lead in both revenue and order volume.

       ✓ Supreme pizzas follow closely, showing strong customer preference.

       ✓ Chicken pizzas have the lowest order volume among all categories.

       ✓ Classic category contributes 26.72% of category sales—the largest share.

       ✓ Demand is concentrated mainly in Classic and Supreme, with Veggie and Chicken categories trailing.

  #### Pizza Size Insights

       ✓ Large pizzas are the most purchased size.

       ✓ Medium pizzas also perform well.

       ✓ X-Large pizzas attract a moderate share.

       ✓ XX-Large pizzas have the least demand.

  #### Best & Worst Sellers

       ✓ Thai Chicken Pizza generates the highest revenue among individual pizzas.

Thai Barbeque Carre Pizza has the lowest revenue.

Classic Deluxe Pizza sells the highest quantity.

Mediterranean Pizza records the lowest quantity sold.

Classic Deluxe Pizza also leads in total orders.

Specialty pizzas like Green, Spinach, and Mediterranean consistently appear in the bottom lists.

Category Breakdown (2015 Panel)

Top-revenue pizzas are dominated by Chicken and Barbecue varieties.

Bottom-quantity pizzas include niche flavors with limited customer adoption.

📈 Recommendations
1. Strengthen Midweek Promotions

Introduce targeted offers on Tuesdays and Wednesdays to lift low-performing days (discounts, bundles, loyalty boosts).

2. Expand Top-Performing Categories

Develop new variations of Classic and Supreme pizzas, as these generate the highest revenue and demand.

3. Reevaluate Low-Demand Items

Reformulate, rebrand, or remove consistently low-performing pizzas such as Mediterranean, Green, and Spinach variants.

4. Promote Large and Medium Size Combos

Since these sizes dominate sales, introduce value deals like family combos or size-based promotions.

5. Apply Seasonal Strategies

Use targeted campaigns:

Summer deals to reinforce July spikes

Fall specials to improve October performance

6. Highlight Best Sellers

Feature top items (Classic Deluxe, Thai Chicken Pizza) prominently in menus, apps, and ordering platforms.

7. Align Inventory With Demand

Increase stock for high-demand ingredients (Classic & Supreme), while reducing overstock of low-selling specialty ingredients.
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
