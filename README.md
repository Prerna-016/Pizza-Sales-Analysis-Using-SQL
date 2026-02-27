# 🍕 Pizza Sales Analysis Using SQL (MySQL)

## 📌 Project Overview

The **Pizza Sales Analysis Using SQL** project focuses on analyzing sales performance, customer preferences, and revenue trends of a pizza restaurant using structured query language (SQL).

This project demonstrates how SQL can be used to extract meaningful business insights from structured relational data. The analysis helps understand customer ordering behavior, top-performing products, and revenue distribution.

---

## 📂 Dataset Information

**Dataset Name:** `Pizza_sales`

The dataset consists of four relational tables:

| Table Name      | Description                                   |
| --------------- | --------------------------------------------- |
| `orders`        | Contains order date and time details          |
| `order_details` | Contains quantity and pizza ID for each order |
| `pizzas`        | Contains pizza size and pricing information   |
| `pizza_types`   | Contains pizza names and categories           |

The tables are connected using primary and foreign key relationships.

---

## 🛠️ Technologies Used

* MySQL
* SQL Joins
* Aggregate Functions (SUM, COUNT, AVG)
* GROUP BY & ORDER BY
* Subqueries
* Window Functions

---

## 📊 Business Problems Solved Using SQL

The following business questions were answered through SQL queries:

1. Retrieve the total number of orders placed.
2. Calculate the total revenue generated from pizza sales.
3. Identify the highest-priced pizza.
4. Determine the most commonly ordered pizza size.
5. List the top 5 most ordered pizza types along with their quantities.
6. Calculate the total quantity of each pizza category ordered.
7. Determine the distribution of orders by hour of the day.
8. Find category-wise distribution of pizzas.
9. Calculate the average number of pizzas ordered per day.
10. Identify the top 3 most ordered pizza types based on revenue.
11. Calculate the percentage contribution of each pizza type to total revenue.
12. Analyze cumulative revenue generated over time.
13. Determine the top 3 most ordered pizza types based on revenue within each category.

---

## 🧮 Sample SQL Query

### Calculate Total Revenue

```sql
SELECT 
    ROUND(SUM(order_details.quantity * pizzas.price), 2) AS total_revenue
FROM order_details
JOIN pizzas 
    ON pizzas.pizza_id = order_details.pizza_id;
```

---

## 📈 Key Insights Derived

* Identified peak business hours for better operational planning.
* Determined top-selling pizza types.
* Analyzed revenue contribution by pizza category.
* Calculated cumulative revenue growth over time.
* Identified high-value products contributing most to total revenue.

---

## 🚀 How to Run This Project

1. Install **MySQL**.
2. Create a new database.
3. Import the dataset tables:

   * `orders`
   * `order_details`
   * `pizzas`
   * `pizza_types`
4. Execute the SQL queries.
5. Analyze the results to derive business insights.

---

## 📁 Project Structure

```
Pizza-Sales-Analysis/
│
├── dataset/
│   ├── orders.csv
│   ├── order_details.csv
│   ├── pizzas.csv
│   └── pizza_types.csv
│
├── SQL_Queries.sql
└── README.md
```

---

## 🎯 Learning Outcomes

* Practical implementation of SQL for business analysis
* Understanding relational database design
* Writing efficient SQL queries using joins and aggregations
* Performing revenue and performance analysis
* Translating raw data into actionable business insights
---
