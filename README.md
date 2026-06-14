# Customer Segmentation Analysis Using RFM

## Project Overview

This project applies RFM (Recency, Frequency, Monetary) analysis to segment customers based on their purchasing behavior. The goal is to identify valuable customer groups, understand customer engagement patterns, and generate business recommendations that can support retention and marketing strategies.

Customer segmentation helps businesses allocate resources more effectively by targeting different customer groups with personalized campaigns instead of treating all customers the same.

---

## Business Problem

Businesses often struggle to understand which customers contribute the most value and which customers are at risk of becoming inactive. Without customer segmentation, marketing efforts may be inefficient and fail to address the specific needs of different customer groups.

This project uses RFM analysis to classify customers into meaningful segments based on transaction recency, purchase frequency, and spending behavior.

---

## Dataset

The analysis uses an online retail transaction dataset containing:

* Customer ID
* Order ID
* Order Date
* Product Code
* Product Name
* Quantity
* Transaction Amount

Each row represents a customer transaction.

---

## Tools and Libraries

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook

---

## Data Cleaning

Several preprocessing steps were performed before the analysis:

* Converted order dates into datetime format.
* Removed records with missing customer IDs.
* Removed records with missing product names.
* Standardized product names into lowercase format.
* Identified cancelled and delivered transactions.
* Cleaned transaction records for further analysis.

---

## Methodology

### 1. Customer Aggregation

Transaction-level data was aggregated into customer-level metrics:

* Total number of orders
* Last purchase date
* Total purchase value

### 2. RFM Calculation

#### Recency

Measures the number of days since the customer's last purchase.

#### Frequency

Measures how many orders a customer has placed.

#### Monetary

Measures the total amount spent by a customer.

### 3. RFM Scoring

Customers were assigned scores from 1 to 5 using percentile-based binning.

### 4. Customer Segmentation

Customers were classified into the following segments:

* Champion
* Loyal Customers
* Potential Loyalists
* New Customers
* Promising
* Need Attention
* About To Sleep
* At Risk
* Can't Lose Them
* Hibernating

---

## Key Findings

### Customer Distribution

The largest customer segments were:

| Segment             | Customers | Percentage |
| ------------------- | --------: | ---------: |
| Hibernating         |     1,060 |      27.3% |
| Champion            |       550 |      14.1% |
| Loyal Customers     |       546 |      14.0% |
| Potential Loyalists |       523 |      13.4% |

### Insights

* Hibernating customers represent the largest customer group, indicating a substantial number of inactive customers that may require re-engagement strategies.
* Champion customers form a strong base of high-value customers who purchase frequently and recently.
* Loyal Customers show strong engagement and have the potential to move into the Champion segment with targeted retention efforts.
* Potential Loyalists represent an opportunity for future growth through increased transaction frequency and personalized marketing campaigns.

---

## Business Recommendations

### Champion

* Offer exclusive rewards and loyalty programs.
* Provide early access to new products.
* Encourage referral programs.

### Loyal Customers

* Implement personalized promotions.
* Increase engagement through loyalty benefits.
* Encourage more frequent purchases.

### Potential Loyalists

* Introduce targeted email campaigns.
* Offer incentives for repeat purchases.
* Promote cross-selling opportunities.

### Hibernating Customers

* Launch customer reactivation campaigns.
* Provide comeback discounts and special offers.
* Develop win-back marketing strategies.

---

## Skills Demonstrated

* Data Cleaning
* Customer Analytics
* Exploratory Data Analysis (EDA)
* RFM Analysis
* Customer Segmentation
* Business Insight Generation
* Data Visualization
* Python Programming

---

## Conclusion

This project demonstrates how RFM analysis can be used to transform transaction data into actionable customer insights. By identifying customer segments based on purchasing behavior, businesses can design more effective retention, engagement, and marketing strategies while maximizing customer lifetime value.
