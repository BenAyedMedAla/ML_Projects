# Customer Segmentation (Clustering)

This project focuses on customer segmentation using clustering techniques. Specifically, we used the **K-Means clustering** algorithm to group customers based on their annual income and spending score. The objective is to categorize customers into different segments to enable targeted marketing strategies.

## Project Overview

Customer segmentation is a common task in business analytics where companies aim to understand customer behavior and tailor their marketing efforts. By using clustering techniques like **K-Means**, we can group customers with similar characteristics, which allows businesses to identify patterns and improve their service offerings.

## Dataset

The dataset used in this project is from the **Mall_Customers.csv** file and contains the following key features:

- **CustomerID**: Unique identifier for each customer.
- **Gender**: Gender of the customer (Male/Female).
- **Age**: Age of the customer.
- **Annual Income (k$)**: The annual income of the customer in thousands of dollars.
- **Spending Score (1-100)**: A score assigned based on the customer's spending behavior.

### Key Features for Clustering:
- **Annual Income**
- **Spending Score**

## Steps Involved

### 1. Data Loading and Exploration

- **Loading the dataset**: The dataset is loaded into a Pandas DataFrame for analysis.
- **Exploratory Data Analysis (EDA)**:
  - Checking the number of customers of each gender.
  - Examining the structure of the data (missing values, data types, etc.).
  - Statistical summary of the dataset (mean, standard deviation, etc.).

### 2. Pre-processing the Data

- **Selecting relevant features**: In this project, we focus on two features: **Annual Income** and **Spending Score**.
- **Handling missing data**: We check for missing values and handle them as necessary.

### 3. Finding the Optimal Number of Clusters

- **Elbow Method**: To determine the optimal number of clusters for K-Means, we use the **Within-Cluster Sum of Squares (WCSS)** method. The "elbow" of the graph helps identify the best number of clusters by plotting the WCSS for different cluster numbers.
- **Optimal number of clusters**: Based on the elbow graph, we determine that the optimal number of clusters is **5**.

### 4. Model Training (K-Means Clustering)

- **K-Means Algorithm**: The K-Means clustering algorithm is applied with 5 clusters. The model is trained using the selected features and the clusters are assigned to each customer.

### 5. Visualizing the Clusters

- **Cluster Visualization**: The resulting clusters are visualized on a scatter plot where:
  - **X-axis** represents **Annual Income**.
  - **Y-axis** represents **Spending Score**.
- The clusters are color-coded for differentiation, and the centroids of each cluster are marked to show the center of each group.

## Results

The customers are grouped into five distinct clusters, each representing a different segment of customers with unique characteristics based on their **Annual Income** and **Spending Score**.

### Cluster Insights:
1. **Cluster 1**: Customers with low income and low spending score.
2. **Cluster 2**: Customers with low income and high spending score.
3. **Cluster 3**: Customers with medium income and medium spending score.
4. **Cluster 4**: Customers with high income and low spending score.
5. **Cluster 5**: Customers with high income and high spending score.

## Conclusion

The K-Means clustering algorithm was successfully used to segment customers based on their income and spending behavior. These insights can be used for personalized marketing campaigns, product recommendations, and improving customer engagement strategies.

## Requirements

- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn