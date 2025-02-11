# Customer Segmentation Analysis using Machine Learning
## Table of Contents
### Introduction
  + Project Description
  +	Key Questions
  + Dataset Overview
### Data Wrangling and Exploration
   + Data Cleaning
   + Feature Engineering
   + Descriptive Statistics
### Customer Segmentation
   + K-Means Clustering
   + Cluster Interpretation
   + Silhouette Score Analysis
### Insights
    + High-Value Customers
    + Engagement Trends
    + Campaign Effectiveness
###  Visualizations
    + Key Charts and Graphs
### Recommendations
    + Marketing Strategies
    + Age-Specific Campaigns
    + Campaign Optimization
### Conclusion
    + Summary of Findings
    + Next Steps






## Introduction

### Project Description:
The aim of this data analytics project is to perform customer segmentation analysis for an e-commerce company. By analyzing customer behavior and purchase patterns, the goal is to group customers into distinct segments. This segmentation can inform targeted marketing strategies, improve customer satisfaction, and enhance overall business strategies.

Key question(s) to guide my Customer Segmentation Analysis:

+ What are the main customer segments based on purchasing behavior?
+ Which factors influence customer engagement in marketing campaigns?
+ How do online vs. offline shoppers differ?
+ What are the characteristics of high-value customers?
+ What are the characteristics of high-value customers?

### Data Description

Dataset Description: Customer Segmentation for E-Commerce firm.
This dataset contains 2,205 rows and 39 columns, representing customer demographic details, purchasing behavior, engagement with marketing campaigns, and overall shopping patterns. The goal of this dataset is to analyze customer segments and derive insights for targeted marketing strategies.

1. Customer Demographics:

ID – Unique identifier for each customer.
Year_Birth – Year of birth of the customer.
Education – Highest level of education (Graduation, PhD, Master, etc.).
Marital_Status – Customer’s marital status (Single, Married, etc.).
Income – Annual income of the customer (in monetary units).
Kidhome – Number of children in the household.
Teenhome – Number of teenagers in the household.

3. Customer Engagement & Tenure:

Dt_Customer – Date when the customer was registered.
Recency – Number of days since the last purchase.
Customer_Days – How long the customer has been with the company (in days).

4. Purchase Behavior:

MntWines – Amount spent on wine products.
MntFruits – Amount spent on fruit products.
MntMeatProducts – Amount spent on meat products.
MntFishProducts – Amount spent on fish products.
MntSweetProducts – Amount spent on sweets.
MntGoldProds – Amount spent on gold products.
MntTotal – Total amount spent on all product categories.
MntRegularProds – Amount spent on regularly purchased products.

5. Purchasing Channels:

NumDealsPurchases – Number of purchases made with discounts.
NumWebPurchases – Number of purchases made through the website.
NumCatalogPurchases – Number of purchases made using a catalog.
NumStorePurchases – Number of purchases made in-store.
NumWebVisitsMonth – Number of visits to the website in the last month.


6. Marketing Campaign Responses:

AcceptedCmp1-5 – Whether the customer accepted offers from five different marketing campaigns (1 = Accepted, 0 = Not Accepted).
AcceptedCmpOverall – Whether the customer accepted at least one campaign.
Response – Whether the customer accepted the last marketing campaign.

7 Additional Features:

Complain – Whether the customer has filed a complaint (1 = Yes, 0 = No).
Z_CostContact, Z_Revenue – Internal company variables (potentially irrelevant).
Potential Use Cases
Customer segmentation: Identifying distinct customer groups based on behavior.
Marketing strategy optimization: Understanding which customers respond to promotions.
Predicting high-value customers: Recognizing patterns in spending behavior.
Product recommendation strategies: Identifying product preferences by segment.
