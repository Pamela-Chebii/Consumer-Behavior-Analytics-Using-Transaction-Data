# **`CONSUMER BEHAVIOR ANALYTICS USING TRANSACTION DATA`**
## **`Project Overview`**

This project analyzes customer purchasing behavior to estimate Customer Lifetime Value (CLV) using transactional data. By modeling customer purchase patterns, the study predicts the expected number of future purchases and the potential revenue each customer may generate.

The analysis applies probabilistic customer behavior models widely used in customer analytics and marketing science.


## **`Methodology`**

The analysis followed a structured data analytics workflow consisting of data preparation, exploratory analysis, machine learning, and customer value estimation.

### **`1. Data Collection`**

The study used the UCI Online Retail II Dataset, which contains transactional records of an online retail store. The dataset includes customer purchases from December 2010 to December 2011 and contains information such as invoice numbers, product descriptions, quantities purchased, transaction dates, prices, and customer identifiers.
### `2. Data Preparation`

Data preprocessing was performed to ensure the dataset was suitable for analysis.

The following steps were carried out:

- Removal of cancelled transactions (Invoices beginning with C)
- Removal of records with missing Customer ID
- Creation of TotalPrice (Quantity × Price)
- Conversion of invoice dates to datetime format
- Aggregation of transactions into customer-level features

Customer-level features were derived using RFM analysis, which includes:

- Recency – number of days since a customer’s last purchase

- Frequency – number of unique transactions made by the customer

- Monetary – total amount spent by the customer

## `3. Exploratory Data Analysis (EDA)`

Exploratory analysis was conducted to understand customer purchasing patterns and data distribution.

This included:

- Distribution analysis of Recency, Frequency, and Monetary values

- Skewness analysis and log transformations

- Correlation analysis using a heatmap

- Visualization of customer behavior patterns