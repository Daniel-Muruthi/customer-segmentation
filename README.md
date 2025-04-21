# Customer Segmentation Using RFM Analysis and KMeans Clustering

## 📌 Project Overview

This project focuses on segmenting customers based on their purchasing behavior using RFM (Recency, Frequency, Monetary) analysis combined with KMeans clustering. The objective is to identify distinct customer groups to enhance targeted marketing strategies and improve customer retention.

## 🎯 Objectives

- Analyze customer purchasing patterns using RFM metrics.
- Segment customers into meaningful groups using KMeans clustering.
- Evaluate the effectiveness of the clustering model.
- Provide strategic recommendations based on customer segments.

## 🗂️ Dataset Description

The analysis utilizes data from two sources:

1. **Online Retail Dataset**:
   - **Time Frame**: 01/12/2010 to 09/12/2011
   - **Description**: Contains transactions for a UK-based online retailer specializing in unique all-occasion gifts.
   - **Size**: Approximately 541,909 records
   - **Source**: UCI Machine Learning Repository

2. **Online Retail II Dataset**:
   - **Time Frame**: 01/12/2009 to 09/12/2011
   - **Description**: Extends the data range, providing a more comprehensive view of customer transactions.
   - **Size**: Approximately 1,067,371 records
   - **Source**: UCI Machine Learning Repository

**Common Features Across Both Datasets**:

- **InvoiceNo**: Unique identifier for each transaction
- **StockCode**: Unique identifier for each product
- **Description**: Product name
- **Quantity**: Number of products per transaction
- **InvoiceDate**: Date and time of the transaction
- **UnitPrice**: Price per unit in sterling (£)
- **CustomerID**: Unique identifier for each customer
- **Country**: Customer's country of residence

## 🛠️ Data Preprocessing

- **Data Cleaning**:
  - Removed duplicate entries and missing values.
  - Filtered out canceled transactions and negative quantities.

- **Feature Engineering**:
  - Calculated RFM metrics for each customer.
  - Applied log transformation to the Monetary value to reduce skewness.

- **Normalization**:
  - Standardized RFM features using `StandardScaler` to ensure equal weighting in clustering.

## 📊 Exploratory Data Analysis (EDA)

- Visualized distributions of RFM metrics to understand customer behavior.
- Identified outliers and patterns in purchasing behavior.
- Assessed correlations between RFM features.

## 🤖 Modeling

- **Clustering Algorithm**: Applied KMeans clustering to the preprocessed RFM data.
- **Evaluation Metrics**:
  - **Silhouette Score**: 0.4433
  - **Davies-Bouldin Index**: 0.7397
- **Cluster Analysis**:
  - Interpreted each cluster based on RFM values.
  - Identified characteristics of high-value and low-value customer segments.

## 📈 Results

- Successfully segmented customers into distinct groups with varying purchasing behaviors.
- High-value customers identified for targeted marketing campaigns.
- Insights gained to inform business strategies and improve customer engagement.

## 📌 Recommendations and Next Steps

- **Marketing Strategies**:
  - Develop personalized marketing campaigns for high-value customer segments.
  - Implement retention strategies for at-risk customer groups.

- **Further Analysis**:
  - Explore additional clustering algorithms for comparison.
  - Incorporate demographic data for more comprehensive segmentation.

- **Business Implementation**:
  - Integrate segmentation results into CRM systems.
  - Monitor customer behavior over time to adjust strategies accordingly.

## 📁 Repository Structure

```
customer-segmentation/
├── index.ipynb               # Main Jupyter Notebook with analysis
├── README.md                 # Project overview and documentation
├── data/                     # Directory containing datasets
│   ├── online_retail.csv
│   └── online_retail_II.csv
├__ customer_segmentation_report.pdf    # Project Report

```

## 📚 References

- [UCI Machine Learning Repository: Online Retail Dataset](https://archive.ics.uci.edu/ml/datasets/Online+Retail)
- [UCI Machine Learning Repository: Online Retail II Dataset](https://archive.ics.uci.edu/ml/datasets/Online+Retail+II)

#### Email: adinomuruthi1@gmail.com