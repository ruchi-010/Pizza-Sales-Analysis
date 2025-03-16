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
