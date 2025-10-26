This project uses the K-Means algorithm to segment customers from the "Mall_Customers.csv" dataset into 5 distinct groups based on their annual income and spending score.

## Project Steps

1.  **Data Loading:** Loaded the `Mall_Customers.csv` dataset.
2.  **Data Preparation:** Selected the 'Annual Income (k$)' and 'Spending Score (1-100)' columns for clustering.
3.  **Data Scaling:** Used `StandardScaler` to scale the features, ensuring that both variables have equal importance for the K-Means algorithm.
4.  **Optimal 'k' Selection:** Used the **Elbow Method** to find the optimal number of clusters. The graph showed a clear "elbow" at **k=5**.
5.  **Clustering:** Applied the K-Means algorithm with n_clusters=5.
6.  **Visualization:** Plotted a 2D scatter plot to visualize the 5 resulting customer segments.

## Analysis of Customer Segments

Based on the visualization, we can identify 5 targetable customer segments:

* **Cluster 0: Standard:** Customers with average income and average spending scores.
* **Cluster 1: Target (High Spenders):** Customers with high income and high spending scores. (This is the prime target group).
* **Cluster 2: Careful:** Customers with low income and low spending scores.
* **Cluster 3: Thrifty:** Customers with high income but low spending scores.
* **Cluster 4: High-Potential:** Customers with low income but high spending scores.

## Marketing Recommendations

* **Cluster 1 (Target):** Engage with loyalty programs, exclusive previews, and premium offers.
* **Cluster 3 (Thrifty):** Target with "premium-for-value" deals or introductory offers to convert their high income into spending.
* **Cluster 4 (High-Potential):** Target with discounts, "buy one get one" offers, and credit options to leverage their high spending behavior.
* **Clusters 0 & 2:** Standard marketing and general promotions.
