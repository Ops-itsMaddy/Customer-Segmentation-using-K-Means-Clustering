**Customer Segmentation using K-Means Clustering**

This repository contains a data science project that implements an Unsupervised Machine Learning model to perform customer segmentation for a retail business. Using the K-Means Clustering algorithm, the model categorizes customers into distinct groups based on their purchasing behavior.

**📊 Project Overview**

The primary objective is to identify different segments within a customer base to enable targeted marketing strategies. The analysis specifically focuses on two key features from the Mall_Customers.csv dataset:

    Annual Income (k$): The yearly income of the customer.

    Spending Score (1-100): A score assigned by the mall based on customer behavior and spending nature.

**🛠️ Tech Stack**

Language: Python

Libraries:

    Pandas & NumPy: For data collection, cleaning, and matrix operations.

    Scikit-Learn: Specifically the KMeans module for cluster analysis.

    Matplotlib & Seaborn: To visualize the elbow graph and the final clusters.

**📑 Implementation Steps**

1. Data Collection & Analysis
The project begins by loading the Mall_Customers dataset containing 200 rows and 5 columns. Initial exploration confirms there are no missing values in the dataset.

2. Finding the Optimal Clusters (k)
To determine the most efficient number of segments, the Elbow Method is used.

    The Within-Cluster Sum of Squares (WCSS) is calculated for various cluster counts (1 through 10).

    A line plot is generated to find the "elbow point," which indicates where adding more clusters no longer significantly improves the model.

3. Training the Model

Based on the elbow graph, the optimum number of clusters is identified as 5. The K-Means model is then initialized with k-means++ to ensure better centroid placement and trained on the features.

4. Visualization
The final step involves plotting the 5 clusters on a 2D scatter plot:

    Each cluster is color-coded for clarity.

    The Centroids (center points) of each cluster are marked in black to show the core characteristic of that segment.

**🚀 How to Use**

Ensure you have the Mall_Customers.csv file in your directory.

Install dependencies: pip install pandas numpy matplotlib seaborn scikit-learn.

Run the Jupyter Notebook to view the step-by-step analysis and resulting visualizations.