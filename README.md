# 2. Power-BI-Sales-Performance-Analysis
Yearly Sales Performance Analysis
 
[View the Power BI Dashboard](https://app.powerbi.com/view?r=eyJrIjoiZDM1YTRjZjEtOGZhYy00OGE2LWE3ZGItZWU0MTc0MDFlN2YxIiwidCI6IjFhOTM4M2ZmLTVlMDEtNDkzYy04MTJmLTg0ODAzZTliMGI3YiJ9)

 ### 1. Domain: Food & Beverage 

# Analysis Details
 ## i. Business Case
 
##### 🚩 Problem Statement:

The pizza business shows strong overall sales, but key performance drivers remain unclear. The company lacks detailed insights into customer behavior, product performance, and demand patterns, making it difficult to optimize operations and maximize revenue.

##### Key Issues:

✔️ Uncertainty about which pizza categories, sizes, and individual items drive the most revenue.

✔️ Inconsistent sales across weekdays and months, with no clear strategy to balance demand.

✔️ Over-dependence on a few top-selling pizzas while many items underperform.

✔️ Inefficient inventory management due to unclear ingredient and product demand trends.

✔️ Limited understanding of seasonal and daily order patterns.

✔️ Missed opportunities to create targeted promotions for low-performing periods.

✔️ Lack of data-driven decision-making to improve menu offerings and reduce waste.

The E-Commerce Sales Analytics Dashboard aims to address several key business challenges related to sales performance, customer behavior, product profitability, and regional growth. Despite generating strong revenue and profit, the organization faces gaps in customer retention, uneven regional performance, and product return issues that impact overall business efficiency. To support data-driven decision-making, the project focuses on identifying underlying issues and converting raw transactional data into meaningful insights.


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

       ✓ Thai Barbeque Carre Pizza has the lowest revenue.

       ✓ Classic Deluxe Pizza sells the highest quantity.

       ✓ Mediterranean Pizza records the lowest quantity sold.

       ✓ Classic Deluxe Pizza also leads in total orders.

       ✓ Specialty pizzas like Green, Spinach, and Mediterranean consistently appear in the bottom lists.

  #### Category Breakdown

       ✓ Top-revenue pizzas are dominated by Chicken and Barbecue varieties.

       ✓ Bottom-quantity pizzas include niche flavors with limited customer adoption.

## 📈 Recommendations
       1. Strengthen Midweek Promotions. They can introduce targeted offers on Tuesdays and Wednesdays to lift low-performing days (discounts, bundles, loyalty boosts).

       2. Expand Top-Performing Categories. It is recommended to develop new variations of Classic and Supreme pizzas, as these generate the highest revenue and demand.

       3. Reevaluate Low-Demand Items. They should reformulate, rebrand, or remove consistently low-performing pizzas such as Mediterranean, Green, and Spinach variants.

       4. Promote Large and Medium Size Combos. Since these sizes dominate sales, introduce value deals like family combos or size-based promotions.

       5. Apply Seasonal Strategies. For Example, use targeted campaigns such as i) Summer deals to reinforce July spikes ii) Fall specials to improve October performance.

       6. Highlight Best Sellers. Feature top items (Classic Deluxe, Thai Chicken Pizza) prominently in menus, apps, and ordering platforms.

       7. Align Inventory With Demand. It is better to increase stock for high-demand ingredients (Classic & Supreme), while reducing overstock of low-selling specialty ingredients.
   
 ## v. Data Source
 
 [Pizza Sales Dataset (Kaggle)](https://www.kaggle.com/datasets/shilongzhuang/pizza-sales)

# A - Analysis Techniques:
## A1 -🍕 Data Preparation

### Understanding the Dataset Structure

The dataset contains 12 key features covering orders, pricing, pizza details, and timestamps.

order_id, order_details_id, and pizza_id uniquely identify orders and items.

Fields like pizza_size, pizza_type, pizza_ingredients, and pizza_name describe product attributes.

### Cleaning & Standardization

✔️ Standardized date/time formats from order_date and order_time.

✔️ Verified price accuracy by ensuring total_price = unit_price × quantity.

✔️ Normalized pizza sizes and types for consistency across the dataset.

✔️ Checked uniqueness and integrity of identifier fields.

### Feature Engineering for Analysis

✔️ Derived new time-based fields (Day, Month, Hour) for trend analysis.

✔️ Aggregated metrics like total revenue, total pizzas sold, and pizzas per order.

✔️ Grouped data by pizza size and category using pizza_type and pizza_size.

✔️ Prepared fields needed for dashboard visuals (best sellers, order trends, category performance).

# B - DAX (Data Analysis Expression)
   ### KPI Measures
                    Average Order value = sum(pizza_sales[total_price])/DISTINCTCOUNT(pizza_sales[order_id]) 
                    Average Pizzas Per Order = sum(pizza_sales[quantity])/DISTINCTCOUNT(pizza_sales[order_id])
                    Total Orders = DISTINCTCOUNT(pizza_sales[order_id])
                    Total Pizzas Sold = sum(pizza_sales[quantity])
                    Total Revenue = sum(pizza_sales[total_price])
   ### Calculated Columns
                    Month = left(pizza_sales[Month Name],3)
                    Order Day = left(pizza_sales[Day Name],3)

 # C - Analyses and Interactivities

 ## Daily and Monthly Trend Analysis

![Pizza Sales Performance Dashboard](https://github.com/Morsshed/2.-Power-BI-Sales-Performance-Analysis/blob/main/Pizza%20Sales%20Performance%20Analysis%201.png?raw=true)

 ## Performance Analysis

 # D - Conclusion
 The Pizza Sales Performance dashboard provides a data-driven foundation for operational, marketing, and menu decisions. By acting on the insights and recommendations, the business can significantly enhance revenue, reduce inefficiencies, and deliver a more customer-centric product offering. This project demonstrates how analytics can turn raw data into actionable business strategy.
                    
