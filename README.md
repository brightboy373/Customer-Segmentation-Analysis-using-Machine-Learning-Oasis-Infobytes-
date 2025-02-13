# Customer Segmentation Analysis Documentation

This document provides a detailed overview of the **Customer Segmentation Analysis** project, including the methodology, insights, and recommendations. This analysis was conducted to segment customers of an e-commerce company based on their behavior and purchase patterns, with the goal of informing targeted marketing strategies and improving customer satisfaction.

---

## Table of Contents
1. [Introduction](#1-introduction)
   - [Project Description](#project-description)
   - [Key Questions](#key-questions)
   - [Dataset Overview](#dataset-overview)

2. [Data Wrangling and Exploration](#2-data-wrangling-and-exploration)
   - [Data Cleaning](#data-cleaning)
   - [Feature Engineering](#feature-engineering)
   - [Descriptive Statistics](#descriptive-statistics)

3. [Customer Segmentation](#3-customer-segmentation)
   - [K-Means Clustering](#k-means-clustering)
   - [Cluster Interpretation](#cluster-interpretation)
   - [Silhouette Score Analysis](#silhouette-score-analysis)

4. [Insights](#4-insights)
   - [High-Value Customers](#high-value-customers)
   - [Engagement Trends](#engagement-trends)
   - [Campaign Effectiveness](#campaign-effectiveness)

5. [Recommendations](#5-recommendations)
   - [Marketing Strategies](#marketing-strategies)
   - [Age-Specific Campaigns](#age-specific-campaigns)
   - [Campaign Optimization](#campaign-optimization)

6. [Visualizations](#6-visualizations)
   - [Key Charts and Graphs](#key-charts-and-graphs)

7. [Conclusion](#7-conclusion)
   - [Summary of Findings](#summary-of-findings)
   - [Next Steps](#next-steps)

---

## 1. Introduction

### Project Description
The goal of this project is to perform **customer segmentation analysis** for an e-commerce company. By analyzing customer behavior and purchase patterns, we aim to group customers into distinct segments. These segments will inform targeted marketing strategies, improve customer satisfaction, and enhance overall business performance.

### Key Questions
1. What are the main customer segments based on purchasing behavior?
2. Which factors influence customer engagement in marketing campaigns?
3. How do online vs. offline shoppers differ?
4. What are the characteristics of high-value customers?

### Dataset Overview
The dataset contains **2,205 rows** and **39 columns**, including:
- **Customer Demographics**: Income, education, marital status, age, etc.
- **Purchase Behavior**: Amount spent on wine, fruits, meat, fish, sweets, and gold.
- **Engagement Metrics**: Number of web visits, store purchases, catalog purchases, etc.
- **Marketing Campaign Responses**: Acceptance of campaigns 1-5.

---

## 2. Data Wrangling and Exploration

### Data Cleaning
- Checked for missing values (none found).
- Converted column names to lowercase for consistency.
- Removed irrelevant columns (`z_revenue`, `z_costcontact`).

### Feature Engineering
- Created new features:
  - **Education**: Categorized as Postgraduates, Graduates, or Undergraduates.
  - **Family Size**: Sum of `kidhome` and `teenhome`.
  - **Marital Status**: Simplified into "Single" or "Partnered."
  - **Age Group**: Categorized as Young Adult, Middle-Aged Adult, Adult, or Senior.
  - **Income Group**: Divided into low, mid, high, and very high based on quartiles.
  - **Engagement Score**: Sum of web purchases, catalog purchases, store purchases, and web visits.
  - **Total Amount Spent**: Sum of spending across all product categories.

### Descriptive Statistics
- Analyzed key metrics:
  - Average income: $48,613.
  - Average total spending: $473.
  - Average engagement score: 16.5.

---

## 3. Customer Segmentation

### K-Means Clustering
- Used **Principal Component Analysis (PCA)** to reduce dimensionality.
- Applied **K-Means clustering** with **4 clusters** (optimal based on silhouette score).

### Cluster Interpretation
1. **Cluster 0**: Moderate income, low spending, low engagement.
   - **Segment**: Cautious Spenders.
2. **Cluster 1**: High income, high spending, high engagement.
   - **Segment**: Premium Customers.
3. **Cluster 2**: Low income, low spending, low engagement.
   - **Segment**: Budget-Conscious Shoppers.
4. **Cluster 3**: High income, high spending, high engagement.
   - **Segment**: Loyal High-Spenders.

### Silhouette Score Analysis
- Best number of clusters: **4** (silhouette score: 0.4740).

---

## 4. Insights

### High-Value Customers
- **Clusters 1 & 3**: High income, high spending, high engagement.
- **Opportunity**: Focus on retention strategies (e.g., VIP programs, personalized marketing).

### Engagement Trends
- **Single Customers**: More engaged than partnered customers.
- **Age Groups**: Young adults are most responsive to campaigns, while seniors prefer traditional methods.

### Campaign Effectiveness
- **Campaign 4**: Most effective, especially among seniors.
- **Campaign 2**: Least effective, needs redesign.

---

## 5. Recommendations

### Marketing Strategies
- **High-Value Customers**: Offer exclusive deals and VIP loyalty programs.
- **Low-Engagement Customers**: Use targeted discounts and personalized email campaigns.

### Age-Specific Campaigns
- **Young Adults**: Focus on social media and gamified offers.
- **Seniors**: Use traditional methods like direct mail and in-store promotions.

### Campaign Optimization
- Double down on **Campaign 4**.
- Redesign **Campaign 2** with better targeting and messaging.

---

## 6. Visualizations
- **Boxplot for Total Amount Spent**: Identified and handled outliers.
- **Income Distribution**: Highlighted income groups.
- **Cluster Visualization**: 2D and 3D plots of clusters.
- **Engagement vs. Spending**: Positive correlation between engagement and spending.

---

## 7. Conclusion

### Summary of Findings
- Identified **4 distinct customer segments** based on income, spending, and engagement.
- High-value customers (Clusters 1 & 3) are the most engaged and responsive to campaigns.
- Single customers and young adults are more engaged than other groups.

### Next Steps
- Implement targeted marketing strategies based on customer segments.
- Monitor campaign performance and refine strategies as needed.
- Explore advanced techniques like RFM analysis for deeper insights.



