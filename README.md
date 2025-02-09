# SQL Capstone Project - Amazon Sales Data Analysis

## Project Overview

This SQL Capstone Project aims to gain insights into Amazon's sales data and understand the factors affecting sales performance across three different branches located in Mandalay, Yangon, and Naypyitaw. By analyzing product, sales, and customer data, we can identify trends and strategies to enhance business performance.

## About the Data

The dataset contains sales transactions from three Amazon branches with the following 17 columns and 1,000 rows:

| Column                | Description                                 | Data Type           |
|-----------------------|---------------------------------------------|---------------------|
| `invoice_id`          | Invoice of the sales made                  | VARCHAR(30)         |
| `branch`              | Branch at which sales were made            | VARCHAR(5)          |
| `city`                | The location of the branch                 | VARCHAR(30)         |
| `customer_type`       | Type of customer                           | VARCHAR(30)         |
| `gender`              | Gender of the customer                     | VARCHAR(10)         |
| `product_line`        | Product line of the product sold           | VARCHAR(100)        |
| `unit_price`          | Price of each product                      | DECIMAL(10, 2)      |
| `quantity`            | Amount of product sold                     | INT                 |
| `VAT`                 | Tax on the purchase                        | FLOAT(6, 4)         |
| `total`               | Total cost of the purchase                 | DECIMAL(10, 2)      |
| `date`                | Date of purchase                           | DATE                |
| `time`                | Time of purchase                           | TIMESTAMP           |
| `payment_method`      | Total amount paid                          | DECIMAL(10, 2)      |
| `cogs`                | Cost of Goods Sold                         | DECIMAL(10, 2)      |
| `gross_margin_percentage` | Gross margin percentage              | FLOAT(11, 9)        |
| `gross_income`        | Gross income                               | DECIMAL(10, 2)      |
| `rating`              | Customer rating                            | FLOAT(2, 1)         |

## Analysis Goals

1. **Product Analysis**: Understand product performance and identify which product lines are performing well and which ones need improvement.
2. **Sales Analysis**: Investigate sales trends, identify factors driving sales, and recommend strategies for increasing sales.
3. **Customer Analysis**: Uncover customer segments, identify their purchasing behavior, and analyze customer profitability.

## Approach Used

### 1. Data Wrangling

- Built a database and created tables to store the data.
- Inspected for missing (NULL) values and replaced them where necessary using appropriate methods.

### 2. Feature Engineering

- **Time of Day**: Added a column to identify sales during the morning, afternoon, and evening to find peak sales periods.
- **Day Name**: Added a column to identify the day of the week on which sales occurred, helping to determine which days each branch performs best.
- **Month Name**: Added a column for the month of the year to assess seasonal sales trends.

### 3. Exploratory Data Analysis (EDA)

Performed analysis to answer the business questions outlined below, gaining insights from the data.

## Business Questions Answered

1. Count of distinct cities in the dataset.
2. For each branch, identify the corresponding city.
3. Count of distinct product lines in the dataset.
4. Most frequently used payment method.
5. Product line with the highest sales.
6. Revenue generated per month.
7. Month with the peak cost of goods sold.
8. Product line with the highest revenue.
9. City with the highest recorded revenue.
10. Product line with the highest VAT.
11. For each product line, classify "Good" or "Bad" based on average sales.
12. Branch exceeding the average number of products sold.
13. Gender most frequently associated with each product line.
14. Average rating for each product line.
15. Sales occurrences by time of day and weekday.
16. Customer type contributing the highest revenue.
17. City with the highest VAT percentage.
18. Customer type with the highest VAT payments.
19. Count of distinct customer types.
20. Count of distinct payment methods.
21. Most frequent customer type.
22. Customer type with the highest purchase frequency.
23. Predominant gender among customers.
24. Gender distribution across each branch.
25. Time of day with the highest customer ratings.
26. Time of day with the highest ratings by branch.
27. Day of the week with the highest average ratings.
28. Day of the week with the highest average ratings by branch.

## Conclusion

This project provides valuable insights into Amazon's sales performance across multiple branches. It identifies key factors such as sales trends, product line performance, customer behavior, and optimal sales periods. The findings can guide future sales strategies and decision-making.
