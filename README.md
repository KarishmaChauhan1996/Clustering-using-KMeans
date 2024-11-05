# K-Means Clustering-Customer Segmentation

This project demonstrates the use of KMeans clustering for segmenting cusomers of a telecom company into distinct clusters based on specified features. The goal is to group data points so that points within a cluster are more similar to each other than to those in other clusters.

**Table of Contents**

Project Overview

Dataset

Dependencies

Exploratory Data Analysis (EDA)

KMeans Clustering Process

Model Evaluation

Results and Interpretation


**Project Overview**

This project applies the KMeans clustering algorithm to group data points based on certain attributes. Clustering is useful in applications such as customer segmentation, image compression, and anomaly detection. In this project, we utilize KMeans to cluster segment the customers, which may help in developing targeted strategies or further predictive analytics.

**Dataset**

1. The dataset contains various features  that help define the clusters. Columns include:
2. Region: Geographic indicator
3. Tenure: Months with service
4. Age: Age in years
5. Marital: Marital status
6. Address: Years at current address
7. Income: Household income in thousands
8. Ed: Level of education
9. Employ: Years with current employer
10. Retire: Retired
11. Gender: Gender
12. Reside: Number of people in household
13. Tollfree: Toll free service (1 - Using, 0 - Not Using)
14. Equip: Equipment rental (1 - Using, 0 - Not Using)
15. Callcard: Calling card service (1 - Using, 0 - Not Using)
16. Wireless: Wireless service (1 - Using, 0 - Not Using)
17. Longmon: Long distance last month Usage
18. Tollmon: Toll free last month Usage
19. Equipmon: Equipment last month Usage
20. Cardmon: Calling card last month Usage
21. Wiremon: Wireless last month Usage
22. Multline: Multiple lines (1 - Using, 0 - Not Using)
23. Voice: Voice mail (1 - Using, 0 - Not Using)
24. Pager: Paging service (1 - Using, 0 - Not Using)
25. Internet: Internet (1 - Using, 0 - Not Using)
26. Callid: Caller ID (1 - Using, 0 - Not Using)
27. Callwait: Call waiting (1 - Using, 0 - Not Using)
28. Forward: Call forwarding (1 - Using, 0 - Not Using)
29. Confer: 3-way calling (1 - Using, 0 - Not Using)
30. Ebill: Electronic billing (1 - Using, 0 - Not Using)
31. Custcat: Customer category

**Dependencies**

Ensure you have the following dependencies installed:

* Python 3.x
* numpy
* pandas
* matplotlib
* seaborn
* scikit-learn

**Exploratory Data Analysis (EDA)**

Before applying KMeans, an exploratory data analysis was performed to understand the structure and distribution of the data. Key steps include:

Data Cleaning: Handling missing values, outliers, and normalization.

**Feature Selection**

Choosing relevant features for clustering using Principal Component Analysis

**KMeans Clustering Process**

Determining the Optimal Number of Clusters:

The Elbow method and Silhouette analysis were used to determine the ideal number of clusters. Both methods help balance the model complexity and cluster cohesion.

**Fitting the Model**
   
The KMeans algorithm was applied to the selected features of the dataset. The key parameters were:

n_clusters: Optimal number determined from the Elbow method.

random_state: Ensures reproducibility.

**Visualizing the Clusters**

After fitting, we plotted the clusters using PCA (Principal Component Analysis) to reduce the data to two dimensions for visualization. This helps in understanding how well-separated the clusters are.

![kmeans](https://github.com/user-attachments/assets/dd04822e-1b63-4501-ae74-66e99e1c28d3)

![kmeanss](https://github.com/user-attachments/assets/ca1cc0eb-fb96-42ad-a659-2ca530d8493f)

**Model Evaluation**

Several metrics were used to assess the clustering performance:

Inertia: Measures within-cluster variance; lower values indicate tighter clusters.

Silhouette Score: Measures how similar an object is to its own cluster compared to other clusters; higher values indicate well-defined clusters.

Cluster Centers: Analyzing the cluster centroids to understand the main characteristics of each cluster.

**Predicting segment for new data**

Based on the evaluation, we identified distinct clusters with specific characteristics. These clusters could represent meaningful segments, such as customer types, product categories, or behavioral groups. The interpretation of these clusters is documented in the results folder.




