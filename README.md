**Fraud Detection in Banking Transactions**

With the growing use of net banking and UPI, fraudulent transactions are on the rise. Manual fraud detection is inefficient, 
so this project uses unsupervised machine learning to automatically detect anomalies and potential fraud in banking data.

**Overview**
Goal: Detect fraud in banking transactions using unsupervised ML.
Dataset: Sourced from Kaggle, contains real bank transaction records.
Challenge: No labeled data, so unsupervised techniques are used.

**Machine Learning Approach**
Since the dataset lacks labeled fraud indicators, unsupervised learning techniques were used to detect anomalies. 
These models learn the normal patterns in transaction data and flag deviations that may indicate fraud.
**Algorithms Used**
Isolation Forest – Isolates anomalies faster; assigns an anomaly score.
One-Class SVM – Learns normal behavior, flags deviations.
K-Means Clustering – Detects outliers based on distance from cluster centroids.
Local Outlier Factor (LOF) – Identifies points with lower density than neighbors.

**Research Methodology**
Each of the four ML models was implemented independently using the same set of features to ensure consistency. 
The models were trained and evaluated on subsets of the data to detect patterns that suggest fraudulent activities.

-->Data Cleaning & Preprocessing
->Feature Selection
-->Model Implementation (Isolation Forest, One-Class SVM, LOF, K-Means)
-->Anomaly Detection & Visualization
-->Model Evaluation (Using Intersection Analysis)
