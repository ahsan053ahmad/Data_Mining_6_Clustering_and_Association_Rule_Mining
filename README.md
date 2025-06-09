# Data_Mining_6_Clustering_and_Association_Rule_Mining

This repository contains an R Markdown assignment that explores two unsupervised learning techniques: **Clustering (K-means)** and **Association Rule Mining**. The project aims to uncover hidden structure in unlabeled data and identify frequent item patterns using real-world datasets.

---

### Business Problem

Many organizations collect large volumes of data without predefined labels or categories. In such scenarios, **unsupervised learning** techniques—such as clustering and association rule mining—can reveal structure, segment customers or products, and uncover actionable patterns.

This assignment demonstrates how clustering can identify natural groupings in data, while association rules uncover meaningful co-occurrence patterns in transactions, which are widely used in areas like retail analytics, recommendation engines, and market basket analysis.

---

### Project Objective

This assignment was structured around two main goals:

1. **Clustering**:
   - Apply **K-means clustering** to group observations based on numerical attributes.
   - Visualize and interpret cluster assignments.
   - Evaluate clustering effectiveness using internal validation methods like **Within-Cluster Sum of Squares (WCSS)** and the **elbow method**.

2. **Association Rule Mining**:
   - Use the **Apriori algorithm** to find frequent itemsets from transactional data.
   - Generate **association rules** with specified support and confidence thresholds.
   - Interpret and visualize strong rules using lift, confidence, and support.

---

### Solution Approach

The project followed a systematic unsupervised learning pipeline:

- **K-means Clustering**:
  - Scaled the data and selected the optimal number of clusters using the elbow method.
  - Applied K-means algorithm using `kmeans()` and evaluated the clusters.
  - Visualized clusters in 2D space using `fviz_cluster`.

- **Association Rule Mining**:
  - Transformed retail transactions into a suitable format using the `arules` package.
  - Used the `apriori()` function to mine frequent itemsets.
  - Generated and pruned rules using `inspect()` and visualized them with `arulesViz`.

---

### Business Value

These techniques have direct applications across industries:

- **Clustering**:
  - Customer segmentation
  - Product grouping
  - Anomaly detection

- **Association Rules**:
  - Market basket analysis
  - Recommendation systems
  - Cross-sell and up-sell insights

They help businesses uncover hidden insights, segment their markets, and make data-driven decisions without labeled data.

---

### Challenges Encountered

- **Choosing the Right Number of Clusters**: Required exploration of WCSS and domain knowledge to interpret results meaningfully.
- **Sparse Transactional Data**: Needed careful preprocessing and pruning to generate actionable rules.
- **Interpretability**: Balancing statistical strength (e.g., lift, confidence) with business interpretability was key.

---

