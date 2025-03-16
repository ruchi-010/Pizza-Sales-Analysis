# Pizza Sales Analysis
A data-driven study of pizza sales leveraging PostgreSQL for analysis and Excel for visualization, to explore sales performance, order patterns, and strategic business opportunities.

![Dashboard](dashboard.jpg)

# Project Overview
- This project meticulously details the end-to-end process of analyzing a substantial dataset comprising over 632,000 pizza sales transactions.
- Leveraging the powerful data management and analytical capabilities of PostgreSQL, the project transformed raw transactional data into actionable business intelligence.
- Key insights into sales trends, customer preferences, and operational performance were then effectively communicated through compelling visualizations using Microsoft Excel, ultimately leading to the formulation of data-driven recommendations.

# Business Context
- In today's competitive food service industry, understanding customer preferences and sales dynamics is crucial for success.
- This project addresses the need for a pizza business to gain a deeper understanding of its sales data to make informed decisions regarding marketing campaigns, inventory management, staffing, and product development.

# Data Description:
The dataset follows a **Snowflake Schema**, meaning the data is normalized into multiple related tables to reduce redundancy and improve efficiency. Fact tables store transactional data, while dimension tables contain descriptive attributes, ensuring a structured and optimized database design.

The analysis is based on a dataset comprising 632,073 records, with each record representing a single pizza order. The dataset includes detailed information such as:

`order_id`: Unique identifier per transaction line.

`date`: The date each order was placed (formatted as mm/dd/yyyy).

`time`: Time-based insights to find peak ordering hours.

`quantity`, `price`: Essential for computing total revenue.

`size`: Pizza size (S, M, L, XL, XXL).

`name`, `category`, `ingredients`: Detailed breakdown of pizza variety.

![Data Model](datamodel.jpg)

# The analytical process
- Data Exploration and Cleaning: Initial exploration to understand the data structure, identify potential missing values or inconsistencies, and perform necessary data cleaning steps.
- Feature Engineering: Creating new relevant features from the existing data, such as extracting the day of the week and month from the date, extracting ordering hours from time and categorizing time into different periods (e.g., lunch, dinner).
- Exploratory Data Analysis (EDA): Utilizing various statistical and visualization techniques to uncover patterns and trends in the data. This included analyzing:
  - Sales volume and revenue trends over time (daily, weekly, monthly).
  - Distribution of orders across different days of the week and day types (weekday vs. weekend).
  - Peak ordering hours throughout the day.
  - Popularity of different pizza sizes and categories.
  - Top-selling pizza names.
  - Revenue generated from different pizza categories and sizes.
- Dashboard Creation: Developing dashboard to effectively communicate the key findings and insights to stakeholders. The dashboard visually represents metrics such as:
  - Total Orders and Quantity
  - Total Revenue
  - Average Order Value
  - Weekday vs. Weekend Revenue
  - Revenue trends by day of the week
  - Monthly Revenue trends
  - Peak Ordering Hours
  - Pizza Category popularity by quantity
  - Pizza Size popularity by quantity
  - Top-selling pizza names by quantity

# Key Findings and Insights
The analysis revealed several crucial insights into pizza sales:
- **Revenue Dominance:** The business generated a significant total revenue of $801,944.7 from the processed orders.
  
- **Weekday Strength:** Weekdays contribute substantially to the overall revenue, with $583,814.65 generated during these days.
  
- **Weekend Surge:** Weekends also represent a significant portion of sales, contributing $218,130.05 in revenue.
  
- **Average Order Value:** The average order value stands at $38.31.
  
- **Friday is King:** Friday consistently shows the highest sales volume and revenue compared to other weekdays, suggesting a potential opportunity for targeted promotions.
  
- **Midweek Consistency:** Sales remain relatively steady throughout the midweek days (Tuesday, Wednesday, Thursday).
  
- **Summer Peak:** The summer months (June, July, August) appear to be the strongest in terms of revenue, while the fall months (September, October, November) show a dip. This seasonality should be considered for inventory planning and marketing efforts.
  
- **Lunch and Dinner Rush:** Peak ordering hours are concentrated around lunchtime (12 PM - 1 PM) and the early evening (6 PM - 8 PM), indicating the need for adequate staffing during these periods.
  
- **Classic Category Leads:** The 'Classic' pizza category is the most popular in terms of quantity sold, followed by 'Supreme', 'Veggie', and then 'Chicken'. The 'Chicken' category appears to lag behind, suggesting potential for exploring new chicken-based offerings or targeted promotions.
  
- **Large and Medium Reign:** Large (L) and Medium (M) are the most preferred pizza sizes, accounting for a significant portion of sales. Extra-large (XL) and extra-extra-large (XXL) sizes have minimal sales, which might warrant a review of their profitability or marketing strategy. Small (S) pizzas also have a relatively low share.
  
- **Top Pizza Performers:** The top 5 most popular pizzas drive a significant portion of the sales, each representing 20% of the top-selling items. These include "The Thai Chicken Pizza", "The Barbecue Chicken Pizza", "The Pepperoni Pizza", "The Classic Deluxe Pizza", and "The Hawaiian Pizza". This highlights the importance of these core menu items.
