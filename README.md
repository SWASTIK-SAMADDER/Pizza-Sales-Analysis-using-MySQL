# Pizza-Sales-Analysis-using-MySQL
## INTRODUCTION:

This project leveraged MySQL's analytical capabilities and strategic SQL operations (including joins), combined with critical thinking, to extract insights for solving business problems within a pizza dataset. The core analysis centered on understanding sales performance in relation to category, revenue generated, customer choices and preferences, and changes over time.

## KEY FEATURES:
1. TIME BASED ORDER ANALYSIS.
2. ORDERS MANAGEMENT.
3. REVENUE ANALYSIS.
4. MOST POPULAR PIZZAS BASED ON PRICE, ORDER, CATEGORY.

## PROJECT GOALS:

Understand Customer Behaviour ,
Optimize Sales Strategies ,
Improve Operational Efficiency,
Drive Revenue Growth.

## DATA DESCRIPTION:
This document outlines the schema for the tables used in a pizza ordering system database.  The database includes 4 csv format datasheets- order_details, orders, pizzas. Pizza_types. The data description is given below-

### `orders`
- **order_id**: Unique identifier for each order.
- **date**: Date the order was placed.
- **time**: Time the order was placed.

### `order_details`
- **order_details_id**: Unique identifier for each order detail.
- **order_id**: References the `order_id` in the `orders` table.
- **pizza_id**: References the `pizza_id` in the `pizzas` table.
- **quantity**: Quantity of the pizza ordered.

### `pizza_types`
- **pizza_type_id**: Unique identifier for each pizza type.
- **name**: Name of the pizza type (e.g., Margherita, Pepperoni).
- **category**: Category of the pizza (e.g., Veggie, Chicken, Supreme).
- **ingredients**: Ingredients in the pizza type.

### `pizzas`
- **pizza_id**: Unique identifier for each pizza.
- **pizza_type_id**: References the `pizza_type_id` in the `pizza_types` table.
- **size**: Size of the pizza (e.g., Small, Medium, Large).
- **price**: Price of the pizza.

## DATA SCHEMA:
A relational database with four tables managing pizza orders, items, and types.
- **Relationships**: One order to many order details; one pizza type to many pizza sizes. Foreign keys ensure data links and integrity. Data schema is prepared in data model view of Power BI.

## KEY PERFORMANCE INDICATORS (KPI):
- **Total Revenue**: Overall sales generated within the analysis period.
- **Number of Orders**: Total count of pizza orders placed.
- **Average Order Value**: Revenue generated per order.
- **Most Ordered Pizza Types (by Quantity)**: Identifying the most popular products based on the number of orders.
- **Top Revenue-Generating Pizza Types** : Identifying the products contributing the most to the total revenue.
- **Order Distribution by Hour**: Understanding when the highest order volumes occur.
- **Most Popular Pizza Size**: Determining the preferred size among customers.
- **Category-wise Revenue Contribution**: Assessing the performance of different pizza categories (e.g., Classic, Supreme, Chicken, Veggie).
- **Cumulative Revenue Over Time**: Tracking the trend of revenue growth.

## FEATURES:
- Identify the most common pizza size ordered.
- List the top 5 most ordered pizza types along with their quantities.
- Determine the distribution of orders by hour of the day.
- Calculate the total quantity of each pizza category ordered.
- Group orders by date and calculate the average number of pizzas ordered per day.
- Determine the top 3 most ordered pizza types based on revenue.
- Analyze cumulative revenue generated over time.

## DATA INSIGHTS:
-  **Strong Sales Volume**:  $817K revenue from 21K+ orders, indicating significant       market demand. 
-  **Daily Average**:  138 pizzas ordered daily, crucial for operational planning. 
-  **Peak Times**: Lunch (12-1 PM) and early evening (4-7 PM) are peak ordering     periods, vital for staffing. A late-night peak was also noted. 
-  **Popular Categories**: Classic pizzas dominate (26.91% revenue, 14K+ units), followed by Supreme (25.46% revenue, 11K+ units). 
-  **Top Pizzas**: Classic Deluxe is most ordered. Barbecue Chicken, Hawaiian, and Pepperoni are also popular. Thai Chicken and Barbecue Chicken are top revenue 
   drivers. 
- **Preferred Size**: Large (L) is the most common size, guiding inventory. XL/XXL are less popular. 
-  **Category Revenue**: Classic, Supreme, Chicken, and Veggie categories significantly contribute to revenue. Chicken, despite fewer options (around 6), shows 
   growth Potential.
-   **Pricing**: Greek Pizza is highest priced; The Brie Carre Pizza among the lowest. 
-  **Underperformance**: XXL pizzas have low order numbers, suggesting a review. 
-  **Revenue Trend**: Consistent growth indicates a healthy business.

 ## RECOMMENDATIONS:
- **Optimize Inventory**: Ensure sufficient stock of popular pizza types (especially Classic, Thai Chicken, and Barbecue Chicken) and the preferred large size.
- **Strategic Promotions**: Develop targeted promotions for off-peak hours and focus on popular categories like Classic and high-revenue generators like Thai 
   Chicken and Barbecue Chicken. Consider boosting the visibility of the Chicken category.
- **Staffing Optimization**: Adjust staffing levels to meet the increased demand during peak lunch and evening hours.
- **Product Portfolio Review**: Consider discontinuing or re-evaluating underperforming products like XXL pizzas. Explore expanding the variety within the popular 
  Chicken pizza category.
- **Customer Engagement**: Leverage the popularity of Classic pizzas and the Large size in marketing campaigns to attract and retain customers.

 ## CONCLUSION:
  These data-driven insights, derived through rigorous SQL analysis and visualization, provide a solid foundation for informed decision-making and strategic initiatives aimed at enhancing pizza sales performance. By analyzing key metrics and relationships between orders, order details, specific pizzas, and pizza types, the project seeks to optimize sales strategies, improve operational efficiency, and enhance understanding of customer preferences within the pizza business.




