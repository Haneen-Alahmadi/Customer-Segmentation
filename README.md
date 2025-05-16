# Customer-Segmentation
### Customer Segmentation by using KMeans



# 🛍️ Customer Segmentation using K-Means Clustering
## This project applies K-Means Clustering to segment customers based on their demographic and spending behavior using the Mall Customer Segmentation dataset. The goal is to help businesses better understand their customer base and enable targeted marketing strategies.


# Dataset

## The dataset used is Mall_Customers.csv, containing the following features:

* CustomerID

* Gender

* Age

* Annual Income (k$)

* Spending Score (1-100)


## Project Workflow

1. Exploratory Data Analysis (EDA)
* Loaded the dataset and displayed its shape, info, and statistical summary.
* Verified data types and checked for missing values.

2. Data Preprocessing
* Label Encoding: Transformed the Gender column into numerical values (0: Female, 1: Male).
* Feature Scaling: Applied StandardScaler to normalize Age, Annual Income, and Spending Score.

3. Elbow Method for Optimal Clusters
* Iteratively applied KMeans with cluster counts from 1 to 10.
* Plotted the inertia_ values to identify the “elbow point” where the error rate decreases more slowly. The optimal number of clusters was found to be 4.

4. Clustering
* Applied KMeans clustering with n_clusters=4.
* Assigned each customer to a cluster and visualized the results using scatter plots.

5. Visualization and Analysis
* Cluster Distribution: Counted and visualized the number of customers in each cluster.
* Spending Behavior: Used box plots to examine spending scores per cluster.
* Age Distribution: Explored age frequency using histograms.
* Gender-Based Analysis: Compared gender distribution across clusters.


# Results & Insights

## Cluster Characteristics:

### Some clusters represented high-income, low-spending customers (possibly savers).
### Others had moderate income, high-spending customers (possibly ideal targets for promotions).
### Young customers tended to appear more frequently in high-spending clusters.
### Gender distribution was relatively balanced across clusters.

## Visualization:

### Clear segmentation was visible in scatter plots based on income and spending score.
### Pie and bar charts highlighted the proportional representation of each cluster.
