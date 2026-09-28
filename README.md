# Project-2-Exploratory-Data-Analysis-EDA
Exploratory Data Analysis (EDA) project using Python and Pandas to analyze data distributions, statistics, trends, and outliers

## Project Overview

This project focuses on performing Exploratory Data Analysis (EDA) on an e-commerce sales dataset using Python. The analysis was conducted to understand the dataset's statistics, distributions, trends, and potential outliers.

The project contains 1,200 orders and 14 original features related to customers, products, pricing, payments, order status, and sales.

## Objectives

* Calculate basic statistics such as mean, median, and count
* Analyze data distributions
* Identify trends and patterns
* Detect potential outliers using the IQR method
* Analyze product revenue
* Examine order status patterns
* Summarize key business observations

## Tools & Technologies

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Google Colab
* Excel

## Dataset Information

* **Total Orders:** 1,200
* **Original Features:** 14
* **Date Range:** 2023–2025
* **Dataset Type:** E-commerce / Sales Data

### Main Features

* OrderID
* Date
* CustomerID
* Product
* Quantity
* UnitPrice
* ShippingAddress
* PaymentMethod
* OrderStatus
* TrackingNumber
* ItemsInCart
* CouponCode
* ReferralSource
* TotalPrice

## Analysis Performed

### 1. Dataset Overview

The dataset structure, number of records, columns, data types, and missing values were examined using Pandas.

The dataset contains 1,200 records across 14 features.

### 2. Basic Statistics

Descriptive statistics were calculated for the numerical variables.

Key results:

* **Total Transactions:** 1,200
* **Quantity Mean:** 2.95
* **Quantity Median:** 3.00
* **Unit Price Mean:** $356.41
* **Unit Price Median:** $364.21
* **Total Order Value Mean:** $1,053.97
* **Total Order Value Median:** $823.62

The difference between the mean and median TotalPrice indicates that the distribution is affected by higher-value orders.

### 3. Outlier Analysis

The IQR method was used to identify potential statistical outliers.

Results:

* **Quantity:** 0 outliers
* **UnitPrice:** 0 outliers
* **ItemsInCart:** 0 outliers
* **TotalPrice:** 8 outliers

The identified TotalPrice outliers were high-value purchases rather than obvious data-entry errors. The maximum TotalPrice observed was approximately $3,456.40.

### 4. Trend Analysis

Monthly sales were calculated by grouping orders by year and month.

A line chart was used to visualize the monthly revenue trend from 2023 to 2025.

The analysis showed that monthly sales generally remained within an approximate range of $40,000–$50,000.

### 5. Product Revenue Analysis

Revenue was grouped by product to compare product performance.

Key observations:

* **Chairs:** approximately $195.6K revenue
* **Printers:** approximately $195.6K revenue
* **Phones:** approximately $151.7K revenue

Chairs and Printers generated the highest revenue among the products analyzed, while Phones generated the lowest revenue.

### 6. Order Status Analysis

Order statuses were examined to understand the distribution of completed and unsuccessful orders.

The analysis showed that:

* Cancelled Orders: 250
* Returned Orders: 247
* Cancelled + Returned: 497 orders
* Approximately 41.42% of all orders were Cancelled or Returned.

This pattern was identified as an important observation for further investigation into fulfillment and customer-retention factors.

## Key Observations

1. The dataset contains 1,200 transactions across 14 features.
2. Customers purchase approximately 3 units per order on average.
3. Total order values are right-skewed because some orders have significantly higher values.
4. Quantity, UnitPrice, and ItemsInCart showed no statistical outliers using the IQR method.
5. Eight statistical outliers were identified in TotalPrice.
6. Monthly revenue remained relatively stable, generally around $40K–$50K.
7. Chairs and Printers generated the highest product-level revenue.
8. Phones generated the lowest product-level revenue among the analyzed products.
9. Cancelled and Returned orders together represented 497 orders, or approximately 41.42% of the dataset.

## Visualizations

The project includes visualizations for:

* Monthly Revenue Trend
* Revenue by Product
* Data Distributions
* Outlier Analysis

These visualizations help make trends and patterns easier to interpret.

## How to Run

This project was developed using Google Colab.

### Using Google Colab

1. Open `EDA_Analysis.ipynb` in Google Colab.
2. Upload `Dataset for Data Analytics (1).xlsx` when prompted.
3. Run the notebook cells from top to bottom.
4. Review the statistical calculations, visualizations, outlier analysis, and observations.

### Local Python Environment

Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn openpyxl
```

Then open the `.ipynb` notebook using Jupyter Notebook, JupyterLab, or another compatible environment.

## Skills Demonstrated

* Exploratory Data Analysis
* Descriptive Statistics
* Mean and Median Analysis
* Outlier Detection
* IQR Method
* Trend Analysis
* Data Visualization
* Revenue Analysis
* Business Data Interpretation
* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn

## Project Status

**Completed — DecodeLabs Virtual Internship Project 2**
