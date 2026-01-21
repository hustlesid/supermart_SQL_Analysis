Supermart Sales Analytics | SQL Project 📊
A comprehensive SQL-based analysis of supermart sales data, exploring patterns across 9,995 transactions, 794 customers, and 1,863 products to derive actionable business insights.

🎯 Project Overview

This project demonstrates advanced SQL querying techniques applied to a real-world retail database. Through 20+ carefully crafted queries, I analyzed sales performance, customer behavior, product profitability, and operational efficiency.

📂 Database Schema

The supermart database consists of 3 normalized tables with **12,652 total records**:

1. **Customer Table** (794 rows)
```
- Customer ID (Primary Key)
- Customer Name
- Segment (Consumer, Corporate, Home Office)
- Age
- Country
- City
- State
- Postal Code
- Region
```

### 2. **Sales Table** (9,995 rows)
```Order Line (Primary Key)
- Order ID
- Order Date
- Ship Date
- Ship Mode
- Customer ID (Foreign Key → Customer)
- Product ID (Foreign Key → Product)
- Sales
- Quantity
- Discount
- Profit
```
### 3. **Product Table** (1,863 rows)
```
- Product ID (Primary Key)
- Category (Furniture, Office Supplies, Technology)
- Sub-Category
- Product Name
```

# Entity Relationship
```
Customer (1) ──→ (M) Sales (M) ←── (1) Product
   794 rows         9,995 rows        1,863 rows
```

## 🔍 Analysis Categories

### 📈 Sales Performance Analysis
1. Total sales by region
2. Sales contribution by customer segment
3. Monthly sales trends
4. Top 5 customers by revenue

### 🏆 Product Analytics
5. Top-selling products by category
6. Total sales per product category
7. Product ranking within categories
8. Subcategory performance analysis

### 💰 Profitability Insights
9. Discount impact on profit margins
10. Top 3 customers by profit per region
11. Running total of profit by customer

### 🚚 Operational Metrics
12. Order distribution by shipping mode
13. Customer distribution by state

### 🎓 Advanced Analytics
14. Cumulative sales tracking (running totals)
15. Moving average of sales (3-order window)
16. Day-over-day sales differences
17. Percent of total sales by region
18. Largest and smallest orders per customer
19. Dense ranking by ship mode

## 💡 Key Business Insights

### 🎯 Discount Strategy
- **High discounts (>50%)**: Result in significant losses
- **Medium discounts (20-50%)**: Barely break even
- **No discount**: Most profitable approach
- **Recommendation**: Implement conservative discount policy

### 📊 Revenue Drivers
- **Top Segment**: Consumer (highest sales volume)
- **Top Category**: Technology (highest revenue)
- **Top Shipping**: Standard Class (5,968 orders - 59.7% of total)

## 🛠️ Technical Skills Demonstrated

### SQL Concepts Applied:
- ✅ **Multi-table JOINs** (INNER JOIN across 3 normalized tables)
- ✅ **Aggregate Functions** (SUM, AVG, COUNT, MAX, MIN)
- ✅ **Window Functions** 
  - RANK() - Product ranking by sales
  - ROW_NUMBER() - Customer ordering
  - DENSE_RANK() - Sales ranking by ship mode
  - LAG() - Day-over-day comparisons
- ✅ **Common Table Expressions (CTEs)** - Complex subqueries
- ✅ **Date Functions** (DATE_TRUNC for monthly aggregation)
- ✅ **CASE Statements** - Discount categorization
- ✅ **Partition By** - Category-wise analysis
- ✅ **Running Totals** - Cumulative calculations
- ✅ **Moving Averages** - Trend analysis
- ✅ **Percentage Calculations** - Contribution analysis

## 📈 Query Complexity Breakdown

| Complexity | Count | Examples |
|------------|-------|----------|
| Basic (Aggregations, GROUP BY) | 8 | Sales by region, Category totals |
| Intermediate (JOINs, Subqueries) | 6 | Top customers, Product rankings |
| Advanced (Window Functions, CTEs) | 6 | Running totals, Moving averages, LAG |

## 🎓 Learning Outcomes

Through this project, I strengthened my ability to:
- Design and execute complex analytical queries
- Optimize query performance across large datasets
- Translate business questions into SQL logic
- Use window functions for advanced analytics
- Extract actionable insights from raw data

## 🔮 Future Enhancements

- [ ] Build interactive dashboard in Power BI/Tableau
- [ ] Add predictive analytics (sales forecasting)
- [ ] Implement customer segmentation using RFM analysis
- [ ] Create stored procedures for automated reporting
- [ ] Perform seasonal trend analysis
- [ ] Add data quality checks and validation queries

## 🤝 Connect With Me

I'm always open to discussing data analytics, SQL optimization, or potential collaborations!
[Email](https://img.shields.io/badge/Email-Contact-red)](mailto:siddhantcs7c@gmail.com)

**If you found this project helpful, please give it a star!**

📝 **Feedback and suggestions are always welcome.**

