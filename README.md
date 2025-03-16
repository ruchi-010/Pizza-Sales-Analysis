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


