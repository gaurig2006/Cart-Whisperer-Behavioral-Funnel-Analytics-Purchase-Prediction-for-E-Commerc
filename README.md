# Cart Whisperer: Behavioral Funnel Analytics & Purchase Prediction for E-Commerce

In the fast-paced world of online shopping, it’s easy to attract clicks — but far harder to convert them into actual purchases. Cart Whisperer is a hands-on data science project that explores how users move through an e-commerce funnel and builds a predictive model to identify which users are most likely to convert.

## Overview

This project tackles one of the biggest challenges in e-commerce: drop-offs during the buying journey. By analyzing real-world user behavior, we aim to:
- Map how users move from viewing to carting to purchasing
- Measure where and why conversions fail
- Predict future purchases based on behavioral signals

It combines data exploration, behavioral segmentation, funnel analytics, and machine learning — all with the goal of helping businesses convert more browsers into buyers.

## Dataset Details

- Source: Kaggle – E-commerce Behavior Data from Multi-Category Store
- Timeframe: October & November 2019
- Total Size: ~4.2 GB  
- Used for this project: A focused sample of 100,000 user events for faster experimentation

## Funnel Insights

Here’s what we found when analyzing the basic shopping funnel:

| Stage | Conversion Rate |
|-------|------------------|
| View to Cart | 3.30% |
| Cart to Purchase | 52.55% |
| View to Purchase | 5.58% |

These numbers reflect how many users drop off early — and how valuable cart-level retargeting could be.

## Predictive Modeling

To take it further, we trained a machine learning model to predict which users are likely to purchase.

- Model Type: Logistic Regression (baseline, interpretable)
- Target Variable: is_purchase (1 = purchase made)
- Performance:
  - Accuracy: 91%
  - Precision (on buyers): 14%
  - F1-score (on buyers): 12%

Due to class imbalance (very few purchases vs. views), we focused on feature engineering and sampling for better balance.

### Engineered Features:
- Total events per user
- Average price of viewed products
- Active session duration
- Number of active days
- Time since first and last interaction

## Visualizations

- Funnel bar chart showing user count drop across stages
- Scatter plot of user activity vs. average price interest
- Time trend analysis of view vs. purchase behavior

## Tools & Technologies

| Area | Tools |
|------|-------|
| Programming | Python |
| Libraries | Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn |
| Platform | Google Colab, GitHub |
| Data Source | Kaggle public dataset |

## Author’s Note

This project blends behavioral psychology with data — trying to answer a very human question with machine logic: what makes someone actually buy something? It’s a foundation for smarter targeting, personalization, and user experience design.

Gauri Gupta
https://www.linkedin.com/in/gauri-gupta-b6973a277/
