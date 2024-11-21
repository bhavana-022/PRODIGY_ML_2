# PRODIGY_ML_2

## Project Overview
This project demonstrates the implementation of the **K-means clustering** algorithm to group customers of a retail store based on their **purchase history**. By clustering customers based on features such as **Age**, **Annual Income**, and **Spending Score**, businesses can gain insights into customer segments for targeted marketing strategies, personalized offers, and product recommendations.

## Problem Statement
the **K-means clustering** algorithm to categorize retail customers into different clusters based on their demographic and purchasing behavior. The dataset contains customer information such as:

- **CustomerID**: Unique identifier for each customer.
- **Gender**: Gender of the customer.
- **Age**: Age of the customer.
- **Annual Income (k$)**: Customer's annual income in thousands of dollars.
- **Spending Score (1-100)**: A score assigned by the retail company based on the customer's spending behavior, where a higher score represents a higher spending frequency.

The main task is to apply the **K-means algorithm** to group customers into meaningful clusters that will help businesses understand purchasing behavior better.

## Features
- Preprocessing the data for missing values and standardization.
- Implementing K-means clustering to group customers into clusters.
- Visualizing the clusters using scatter plots to represent customer segments.
- Evaluating cluster effectiveness using the **Elbow method** to determine the optimal number of clusters.

## Requirements
- Python 3.x
- numpy
- pandas
- scikit-learn
- matplotlib

You can install the required dependencies using the following command:

```bash
pip install -r requirements.txt
```
## Data
The dataset contains customer details such as **CustomerID**, **Gender**, **Age**, **Annual Income (k$)**, and **Spending Score (1-100)**. Example:

| CustomerID | Gender | Age | Annual Income (k$) | Spending Score (1-100) |
|------------|--------|-----|---------------------|------------------------|
| 1          | Male   | 19  | 15                  | 39                     |
| 2          | Male   | 21  | 15                  | 81                     |
| 3          | Female | 20  | 16                  | 6                      |
| 4          | Female | 23  | 16                  | 77                     |
| 5          | Female | 31  | 17                  | 40                     |
| 6          | Female | 22  | 17                  | 76                     |
| 7          | Female | 35  | 18                  | 6                      |
| 8          | Female | 23  | 18                  | 94                     |
| ...        | ...    | ... | ...                 | ...                    |

This data will be used to segment customers into different clusters based on their income and spending patterns.

### Result:
After applying the KMeans clustering algorithm with 5 clusters, the customers are grouped based on their Annual Income and Spending Score. The clustering result is visualized in a scatter plot where:

- Each data point represents a customer.
- The x-axis shows the Annual Income (k$).
- The y-axis shows the Spending Score (1-100).
- Different colors represent distinct customer clusters.
- The red "X" markers indicate the centroids (centers) of each of the 5 clusters.
### Accuracy:
Since KMeans is an unsupervised learning algorithm, it doesn't calculate accuracy in the conventional sense (like in classification tasks). Instead, KMeans aims to minimize the Within-Cluster Sum of Squares (WCSS), which measures the compactness of the clusters.
