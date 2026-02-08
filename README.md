Customer Churn Analysis – Power BI Dashboard
Author
-Subiksha T

Project Overview

This project analyzes customer churn behavior for a telecom company using Power BI. The objective is to identify patterns, key churn drivers, and high-risk customer segments so the business can take preventive retention actions.

The dashboard provides insights into customer tenure, contract types, spending patterns, and behavioral factors influencing churn.

Problem Statement

A telecom company has observed a decline in active customers, affecting monthly revenue. Management suspects that contract type, tenure, and spending influence churn, but lacks clear insights.

The goal of this project is to:

Analyze customer behavior

Identify churn patterns

Determine key churn drivers

Provide actionable insights for retention strategies

Tools Used

Power BI Desktop – Data visualization and dashboard creation

DAX (Data Analysis Expressions) – Churn rate calculation

Excel/CSV Dataset – Customer churn data

Dataset Features

The dataset includes the following key attributes:

CustomerID

Gender

Age

Tenure

Contract Length

Subscription Type

Support Calls

Payment Delay

Usage Frequency

Total Spend

Churn (0 = No, 1 = Yes)

Key Dashboard Visuals

The Power BI dashboard includes:

Churn Rate Card – Overall churn percentage

Churn Distribution Pie Chart – Churn vs non-churn customers

Tenure Distribution Chart – Customer tenure patterns

Contract Length vs Churn – Churn by contract type

Total Spend vs Churn – Spending behavior of churned customers

Gender vs Churn – Demographic churn comparison

Subscription Type vs Churn – Plan-based churn trends

Support Calls vs Churn – Customer service impact on churn

DAX Measure Used

Churn rate was calculated using the following DAX formula:

Churn Rate =
DIVIDE(
    CALCULATE(
        COUNTROWS('customer_churn_dataset-training-master'),
        'customer_churn_dataset-training-master'[Churn] = 1
    ),
    COUNTROWS('customer_churn_dataset-training-master')
)

Key Insights

Customers with shorter tenure show higher churn rates.

Month-to-month contracts have the highest churn.

Customers with lower total spend tend to churn earlier.

Higher support call frequency is linked to increased churn.

Certain subscription types show higher churn risk.

High-Risk Customer Segment

Customers most likely to churn:

Short tenure

Month-to-month contracts

Higher support interactions

Lower overall spending

Business Recommendations

Based on the analysis:

Offer discounts for long-term contracts.

Provide loyalty rewards for new customers.

Improve customer support quality.

Introduce personalized retention offers for high-risk users.

How to Use the Dashboard

Open the Power BI (.pbix) file.

Use the Gender and Contract Length slicers.

Explore churn patterns across different customer segments.

Project Outcome

This dashboard helps the telecom company:

Identify churn-prone customers

Understand key churn drivers

Take proactive retention actions

Improve customer lifetime value
