E-Commerce Sales Performance Dashboard
Project Overview

The E-Commerce Sales Performance Dashboard is an interactive Business Intelligence project developed using Microsoft Power BI.

The dashboard analyzes e-commerce sales, customers, products, and customer behavior data. It converts raw datasets into interactive visual reports and KPIs that help understand business performance and identify useful trends and patterns.

The project contains multiple dashboard pages for Executive Overview, Sales Performance, Customer Intelligence, Product Analytics, Customer Behavior, and Advanced Analytics.

Objectives
Analyze overall e-commerce sales performance.
Track important business KPIs.
Analyze revenue by different categories and factors.
Understand customer characteristics and purchasing behavior.
Identify high-performing products.
Analyze customer interactions such as views, likes, and purchases.
Calculate important business metrics.
Create an interactive and easy-to-understand dashboard.
Generate insights that can support business decisions.
Tools & Technologies
Microsoft Power BI
Power Query
DAX
Data Visualization
Data Cleaning & Transformation
CSV Dataset
Dashboard Pages
1. Executive Overview

Provides a quick summary of the entire e-commerce business.

KPI Cards
Total Revenue
Total Orders
Total Products
Average Previous Purchases
Average Review Rating
Visualizations
Revenue by Category
Revenue by Location
Payment Distribution
Revenue Trend
2. Sales Performance

Analyzes different factors affecting sales.

Visualizations
Sales by Season
Sales by Gender
Sales by Shipping Type
Discount Impact
Purchase Frequency
Sales by Size
3. Customer Intelligence

Analyzes customer characteristics and customer segments.

Visualizations
Customers by Gender
Customers by Age Group
Subscription Status
Customers by Location
Customer Age vs Revenue
Review Rating Distribution
4. Product Analytics

Analyzes product-level performance.

Visualizations
Top 10 Products
Revenue by Product Category
Product Price Distribution
Stock by Category
Top Brands
Product Rating
5. Customer Behavior

Uses the e-commerce interaction dataset to understand customer activity.

KPI Cards
Total Views
Total Likes
Total Purchases
Conversion Rate
Visualizations
Views vs Purchases
User Interaction Trend
Most Viewed Products
Most Purchased Products
Interaction Distribution
Views → Likes → Purchases
6. Advanced Analytics

Provides deeper analysis and business insights.

Visualizations
Age vs Revenue
Selling Price vs Revenue
Rating vs Revenue
Discount vs Revenue
Subscription vs Revenue
Purchase Frequency vs Revenue
Key Influencers
Basic Operations Used in the Project

These are important concepts you should understand for your viva/interview.

1. Sum

Adds numerical values.

Example:

Total Revenue = SUM(Total Revenue)

Used for:

Total Revenue
Total Stock
Sales
2. Count

Counts the number of records.

Example:

Total Orders = COUNT(Customer ID)

Used for:

Total Orders
Number of customers
Number of products
3. Average

Calculates the mean value.

Example:

Average Rating = AVERAGE(Review Rating)

Used for:

Average Review Rating
Average Previous Purchases
Average Selling Price
4. Minimum

Finds the smallest value.

Example:

Minimum Selling Price
5. Maximum

Finds the largest value.

Example:

Maximum Selling Price
6. Distinct Count

Counts unique values only.

For example:

Customer ID:
1001
1002
1001
1003

Normal count = 4

Distinct count = 3

This is useful when you want the actual number of unique customers.

Data Cleaning

Power BI's Power Query was used for preparing the datasets.

Basic operations include:

Removing empty columns
Removing duplicate records
Handling missing values
Changing data types
Renaming columns
Filtering unnecessary records
Splitting columns
Merging data where required
Replacing incorrect values
DAX

DAX (Data Analysis Expressions) is the formula language used in Power BI for creating calculations and measures.

Example:

Total Revenue =
SUM(customer_details[Total Revenue])

Example:

Average Rating =
AVERAGE(customer_details[Review Rating])
Conversion Rate
Conversion Rate =
DIVIDE(
    CALCULATE(
        COUNTROWS(ecommerce_interactions),
        ecommerce_interactions[Interaction type] = "purchase"
    ),
    CALCULATE(
        COUNTROWS(ecommerce_interactions),
        ecommerce_interactions[Interaction type] = "view"
    ),
    0
)
Interactive Features

The dashboard provides:

Interactive filters
Slicers
Cross-filtering
Drill-down
Page navigation
KPI cards
Interactive charts
Home navigation buttons

Users can select a category, location, season, gender, etc., and the dashboard updates accordingly.

Key Business Insights

The dashboard can help identify:

Which categories generate the most revenue.
Which locations have stronger sales.
Which products perform best.
Which seasons have higher sales.
Which payment methods are commonly used.
How customers differ by age and gender.
How subscription status relates to purchasing.
Which products receive the most interactions.
The relationship between product views and purchases.
Factors associated with higher revenue.
Project Workflow
Raw Dataset
     ↓
Data Import
     ↓
Data Cleaning
     ↓
Data Transformation
     ↓
Data Modeling
     ↓
DAX Calculations
     ↓
KPI Creation
     ↓
Charts & Visualizations
     ↓
Interactive Dashboard
     ↓
Business Insights
