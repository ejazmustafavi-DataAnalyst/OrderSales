# Order Sales Analysis Using SQL

## Project Overview

This project demonstrates SQL data analysis on an e-commerce orders dataset. The objective is to extract meaningful business insights using fundamental SQL operations such as filtering, sorting, grouping, and aggregation.

The analysis was performed using MySQL Workbench on a dataset containing 1,200 customer orders.

## Objectives

- Analyze sales and order data using SQL.
- Practice SQL fundamentals.
- Generate business insights from transactional data.
- Demonstrate the use of aggregation and grouping functions.

## Dataset Information

Columns:
- OrderID
- Date
- CustomerID
- Product
- Quantity
- UnitPrice
- ShippingAddress
- PaymentMethod
- OrderStatus
- TrackingNumber
- ItemsInCart
- CouponCode
- ReferralSource
- TotalPrice

Dataset Size:
- 1,200 Records
- 14 Columns

## Technologies Used

- MySQL
- MySQL Workbench
- Microsoft Excel
- SQL

## SQL Concepts Covered

### SELECT
```sql
SELECT * FROM Orders;
```

### WHERE
```sql
SELECT *
FROM Orders
WHERE TotalPrice > 2000;
```

### ORDER BY
```sql
SELECT *
FROM Orders
ORDER BY TotalPrice DESC;
```

### GROUP BY
```sql
SELECT Product,
       SUM(TotalPrice) AS TotalSales
FROM Orders
GROUP BY Product;
```

### Aggregate Functions
```sql
SELECT COUNT(*) AS TotalOrders FROM Orders;
SELECT SUM(TotalPrice) AS TotalRevenue FROM Orders;
SELECT AVG(TotalPrice) AS AverageOrderValue FROM Orders;
```

## Business Questions Answered

1. How many orders were processed?
2. What is the total revenue generated?
3. What is the average order value?
4. Which products sold the most?
5. Which payment method generated the highest revenue?
6. Which referral source generated the most sales?
7. What is the distribution of order statuses?

## Key Findings

- Total Orders: 1,200
- Total Revenue: 1,264,761.96
- Average Order Value: 1,053.97
- Best-Selling Product: Chair
- Highest Revenue Payment Method: Credit Card
- Best Referral Source: Instagram
- Most Common Order Status: Cancelled

## Project Structure

```text
OrderSales/
├── OrdersData.xlsx
├── schema.sql
├── queries.sql
├── project_report.md
└── README.md
```

## How to Run

1. Create a database in MySQL Workbench.
2. Create the Orders table using the schema script.
3. Import the dataset.
4. Execute the SQL queries.
5. Review the generated insights.

## Conclusion

This project demonstrates the practical application of SQL for data analysis. By using SQL queries and aggregation functions, valuable insights were extracted from customer order data, helping identify sales trends, product performance, payment preferences, and marketing effectiveness.

## Author

Ejaz Mustafavi
Data Analyst | SQL | Excel | Power BI