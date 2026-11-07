# 🛒 ClusterCart
## AI-Powered Customer Segmentation and Behaviour Analysis System

**Discover Customers. Decode Behaviour. Drive Smarter Decisions.**

ClusterCart is an Unsupervised Machine Learning project designed to analyze e-commerce customer data and identify meaningful customer segments based on demographics, purchasing behaviour, shopping preferences, and engagement patterns.

The project uses clustering algorithms to discover hidden patterns in customer behaviour and help businesses make data-driven decisions for personalized marketing, customer engagement, and customer retention.

---

## 📌 Table of Contents

1. Project Overview
2. Problem Statement
3. Project Objectives
4. Dataset Description
5. Technologies Used
6. Project Workflow
7. Data Preprocessing
8. Feature Engineering
9. Exploratory Data Analysis
10. Machine Learning Algorithms
11. Dimensionality Reduction
12. Optimal Cluster Selection
13. Model Implementation
14. Cluster Analysis
15. Project Results
16. Project Structure
17. Installation and Setup
18. Future Improvements
19. Applications
20. Author

---

## 1. 📖 Project Overview

SmartCart is an e-commerce platform serving customers across multiple countries. It collects customer information related to demographics, purchasing habits, website activity, and customer feedback.

ClusterCart transforms this customer information into meaningful groups using Unsupervised Machine Learning.

Instead of treating every customer equally, the system identifies customers with similar characteristics and purchasing patterns.

The project applies:

- K-Means Clustering
- Agglomerative Clustering
- Principal Component Analysis (PCA)
- Elbow Method
- Silhouette Score

The final objective is to understand customer behaviour and support smarter business decisions.

## 2. 🎯 Problem Statement

SmartCart currently uses generic marketing and customer engagement strategies for all customers without clearly understanding their individual behaviour patterns.

This creates several business challenges:

- Inefficient marketing strategies.
- Missed opportunities to retain high-value customers.
- Difficulty identifying different purchasing patterns.
- Delayed identification of customers who may be at risk of leaving.
- Lack of personalized customer engagement.

To solve these challenges, ClusterCart uses Unsupervised Machine Learning to analyze historical customer transaction data and group customers into meaningful clusters based on purchasing behaviour, engagement levels, and loyalty indicators.

## 3. 🚀 Project Objectives

The main objectives of ClusterCart are:

- Analyze customer demographics and purchasing behaviour.
- Identify hidden patterns in customer transaction data.
- Perform data cleaning and preprocessing.
- Handle missing values and outliers.
- Create meaningful features using feature engineering.
- Apply categorical encoding and feature scaling.
- Reduce data dimensions using PCA.
- Determine the optimal number of clusters.
- Implement K-Means Clustering.
- Implement Agglomerative Clustering.
- Compare and visualize customer groups.
- Generate insights to support personalized marketing and customer retention.

## 4. 📊 Dataset Description

The project uses a customer dataset containing:

- Total Records: 2,240
- Total Attributes: 22
- Missing Values: 24 in the Income column

Each row represents an individual customer.

### Dataset Features

### A. Customer Demographics

| Feature | Description |
|---|---|
| ID | Unique customer identifier |
| Year_Birth | Year of birth of the customer |
| Education | Highest education level achieved |
| Marital_Status | Marital status of the customer |
| Income | Yearly household income |
| Kidhome | Number of small children in household |
| Teenhome | Number of teenagers in household |
| Dt_Customer | Date when customer enrolled with SmartCart |

### B. Purchase Behaviour (Amount Spent)

| Feature | Description |
|---|---|
| MntWines | Amount spent on wine products |
| MntFruits | Amount spent on fruits |
| MntMeatProducts | Amount spent on meat products |
| MntFishProducts | Amount spent on fish products |
| MntSweetProducts | Amount spent on sweet products |
| MntGoldProds | Amount spent on gold products |

### C. Purchase Behaviour (Frequency)

| Feature | Description |
|---|---|
| NumDealsPurchases | Purchases made using discounts |
| NumWebPurchases | Purchases made through website |
| NumCatalogPurchases | Purchases made through catalog |
| NumStorePurchases | Purchases made in physical stores |
| NumWebVisitsMonth | Number of visits to website per month |

### D. Customer Feedback and Response

| Feature | Description |
|---|---|
| Recency | Number of days since last purchase |
| Complain | Customer complained in last 2 years (1 = Yes, 0 = No) |
| Response | Customer response indicator available in the CSV dataset |

## 5. 🛠️ Technologies and Libraries Used

### Programming Language
- Python

### Data Analysis
- Pandas
- NumPy

### Data Visualization
- Matplotlib
- Seaborn

### Machine Learning
- Scikit-learn
- K-Means Clustering
- Agglomerative Clustering
- Principal Component Analysis (PCA)
- StandardScaler
- OneHotEncoder

### Additional Library
- Kneed

### Development Environment
- Jupyter Notebook
- Google Colab (compatible environment)

## 6. 🔄 Project Workflow

The complete machine learning workflow follows these steps:

1. Data Collection
2. Data Loading
3. Data Exploration
4. Missing Value Handling
5. Feature Engineering
6. Feature Selection
7. Outlier Detection and Removal
8. Correlation Analysis
9. Categorical Encoding
10. Feature Scaling
11. Dimensionality Reduction using PCA
12. Optimal Cluster Selection
13. K-Means Clustering
14. Agglomerative Clustering
15. Cluster Visualization
16. Customer Segmentation Analysis

## 7. 🧹 Data Preprocessing

Data preprocessing prepares the raw dataset for machine learning.

### Step 1: Data Loading

The dataset is loaded using Pandas.

```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

df = pd.read_csv("smartcart_customers.csv")
