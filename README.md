# Customer Retention Cohort Analysis (E-commerce)
   ## Project Overview

This project performs a Customer Retention Cohort Analysis on an e-commerce transactional dataset to understand customer loyalty, churn patterns, and repeat purchase behavior over time.
Customers are grouped into cohorts based on the month of their first purchase, and retention is tracked monthly to identify how long customers continue buying after their initial transaction.

######  Business Objective

* Measure customer retention over time
* Identify periods of high churn
* Compare performance of different customer cohorts
* Support data-driven retention and marketing strategies


######  Data Cleaning & Preparation

The following steps were applied:

* Removed transactions with missing CustomerID
* Converted InvoiceDate to datetime format
* Removed invalid transactions (negative quantity or price)

Created:

* CohortMonth (first purchase month)
* TransactionMonth
* CohortIndex (months since first purchase)
* Revenue (Quantity × UnitPrice)

 ###### Methodology
* Assign each customer to a cohort based on their first purchase month
* Track customer activity in subsequent months
* Count unique active customers per cohort per month
* Calculate retention rate as a percentage of the original cohort size
* Visualize results using a retention heatmap

######  Key Findings & Interpretation
 * Early Churn Is High
* Across all cohorts, 75–85% of customers churn after their first purchase
* Month-2 retention typically ranges between 15% and 25%
* Retention Stabilizes After Month 3
* Customers who return beyond Month 3 show consistent repeat behavior
* Indicates a smaller but loyal customer base

######  Strongest Cohort Performance

* December 2010 cohort shows the highest long-term retention
* Retention peaks at around 50% by Month 12
* Likely driven by seasonal shopping and promotions

###### Business Recommendations

1. Improve first-month onboarding and follow-ups
2. Introduce incentives for second purchases within 30 days
3. Focus retention spend on high-value seasonal cohorts
4. Re-evaluate customer acquisition strategies for weaker cohorts

###### Skills Demonstrated

* Python (Pandas, NumPy)
* Cohort analysis & retention metrics
* Data cleaning & transformation
* Data visualization (Matplotlib, Seaborn)
* Business insight generation
