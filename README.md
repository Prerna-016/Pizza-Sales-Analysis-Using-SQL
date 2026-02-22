📊 Project Overview
The primary goal of this project is to analyze the sales performance of a pizza restaurant. By leveraging MySQL, I processed four different datasets to identify trends in customer behavior, revenue generation, and product popularity.

🛠️ Tech Stack
Database: MySQL

Tool: MySQL Workbench

Language: SQL (Structured Query Language)

Concepts Used: Joins, Subqueries, CTEs, Window Functions, Aggregate Functions, and Data Modeling.

📂 Dataset Description
The analysis is based on four CSV files:

Orders: Contains order_id, date, and time for every transaction.

Order Details: Contains order_details_id, order_id, pizza_id, and quantity.

Pizzas: Contains pizza_id, pizza_type_id, size, and price.

Pizza Types: Contains pizza_type_id, name, category, and ingredients.

🚀 Key Analysis & Insights
The project is divided into three levels of complexity:

1. Basic Level
Total Orders: Calculated the total volume of orders placed.

Total Revenue: Summed the total sales generated across all categories.

Pricing Analysis: Identified the highest-priced pizza.

Quantity Trends: Identified the most common pizza size ordered by customers.

2. Intermediate Level
Category Distribution: Analyzed the distribution of pizza orders by category.

Peak Hours: Determined the distribution of orders by the hour of the day to identify peak business hours.

Customer Preferences: Found the top 5 most ordered pizza types based on quantity.

Average Daily Sales: Calculated the average number of pizzas ordered per day using subqueries.

3. Advanced Level
Revenue Contribution: Calculated the percentage contribution of each pizza category to the total revenue.

Cumulative Revenue: Analyzed the cumulative revenue generated over time to track business growth.

Category Ranking: Used window functions to find the top 3 most ordered pizza types based on revenue for each specific category.

📉 Key Findings
Peak Activity: Business peaks between 12:00 PM – 1:00 PM and 4:00 PM – 7:00 PM.

Top Earners: While "Classic" pizzas are the most frequent, the "Thai Chicken Pizza" is a major revenue driver.

Category Leader: The "Classic" category contributes approximately 26.9% of the total revenue.

📖 How to Use
Clone the Repository:

Bash
git clone https://github.com/your-username/pizza-sales-sql-analysis.git
Import Data: Load the provided CSV files into your MySQL environment.

Run Queries: Execute the SQL script provided in this repository to replicate the analysis.
