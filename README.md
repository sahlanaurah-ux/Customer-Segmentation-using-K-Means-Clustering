# Customer Segmentation using K-Means Clustering

A Python project that groups mall customers into segments based on how much they earn and how much they spend. The segments can help a store plan targeted offers and marketing.

Built with Python, Pandas, scikit-learn, Matplotlib and Seaborn. Developed with help from Claude.

## What it does

- Loads the Mall Customers dataset (200 customers).
- Checks the data shape, column types and missing values. There are no missing values.
- Uses two features: **Annual Income (k$)** and **Spending Score (1-100)**.
- Runs K-means for 1 to 10 clusters and plots the WCSS (elbow method) to choose the number of clusters.
- Fits K-means with **5 clusters** and assigns each customer to a segment.
- Plots the five customer groups and their centroids.

## Dataset

The Mall Customers dataset, available on Kaggle. Each row is one customer.

| Column | Meaning |
| --- | --- |
| `CustomerID` | Customer number |
| `Gender` | Male or Female |
| `Age` | Age in years |
| `Annual Income (k$)` | Yearly income in thousands of dollars |
| `Spending Score (1-100)` | Score given by the mall based on spending behavior |

Only income and spending score are used for clustering.

## How it works

1. Select the income and spending score columns.
2. For each number of clusters from 1 to 10, fit K-means and record the WCSS (`inertia_`).
3. Plot WCSS against the number of clusters and pick the elbow point, which is 5 clusters here.
4. Fit the final K-means model with `init='k-means++'` and 5 clusters.
5. Plot each cluster in a different color with the centroids marked.

## How to run

1. Install the libraries:
   ```
   pip install numpy pandas matplotlib seaborn scikit-learn
   ```
2. Download `Mall_Customers.csv` and update the file path in the notebook.
3. Open the notebook in Jupyter and run the cells in order.

## Results

<!-- Add a screenshot of the elbow graph and the customer groups plot here, and a one-line description of each of the 5 groups. -->

## Author

Sahla Nawra V.P.
[LinkedIn](https://www.linkedin.com/in/sahla-nawra-978242273) | [GitHub](https://github.com/sahlanaurah-ux)
