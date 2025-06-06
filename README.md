# Fraud-detection-on-Finance-data


Fraudulent activities are more prevalent in banking sector.
As net banking and UPI transactions are more commonly
used now there is high risk of fraud transaction and money
laundering. Manually identifying and detecting fraud
activities can be more challenging. This requires more
advanced approach like machine learning and data analysis
to classify the fraud data. Machine learning (ML) algorithms
provides solution by regression or classification to identify
actual anomalies and predict fraudulent behavior.

Identifying anomalies in bank dataset can be done using
supervised machine learning algorithm if the dataset contains
labeled data and if the dataset does not contain labeled data
column, unsupervised algorithm like k means , random forest
and more algorithms can be used.

Unsupervised techniques, including clustering and anomaly
detection algorithms, identify unusual patterns in unlabeled
data, highlighting potential fraudulent activities.

The machine learning algorithms utilized in this project are trained to
detect underlying fraud patterns within the data with a high degree of
accuracy. In order to check the accuracy of the model and the
anomalies identified, ensemble methods are used.

ALGORITHMS UTILIZED

In this project, four machine learning algorithms were applied to detect
anomalies and fraudulent transactions in the dataset. These algorithms
include,

    -->One class SVM
    -->Local outlier factor
    -->K-means clustering
    -->Isolation forest

**K-Means Clustering**
K-Means is an unsupervised machine learning algorithm for clustering
data into distinct groups. K-Means algorithm identifies anomalies by
clustering similar transactions together and identifying transactions
that do not belong to any such cluster.
K means clustering algorithm works by
Organizes transactions into K clusters on the basis of similarity.
The value of k is determined by using silhouette method and elbow
method.
It takes into account the distance between each transaction and the
cluster centroids.
The data points with highest distance is marked as anomalies.
Unsupervised machine learning algorithms are used as the data set
does not contain any labeled data. Each algorithm was chosen for its
ability to identify unusual transaction patterns and detect fraudulent
activities effectively.

**One-Class SVM (Support Vector Machine)**
One-Class SVM is a unsupervised anomaly detection algorithm that
learns the characteristics of normal transactions and identifies
deviations from the norm.

**Isolation Forest**
Isolation Forest algorithm isolates the outliers in a dataset by
randomly partitioning the data.
Fraudulent transactions that is anomalies, are isolated faster than
normal transactions. The algorithm assigns an anomaly score, where
higher scores indicate potential fraud.

LOF is a density-based anomaly detection algorithm that identifies
transactions that deviate significantly from their local neighborhood.
It Works by measuring the local density of data points by comparing
them with their nearest neighbors.
Transactions with significantly lower density compared to their
neighbors are considered anomalies.
LOF assigns an outlier score to each transaction, where higher scores
indicate higher fraud probability.
Local Outlier Factor (LOF)

This project follows a structured machine learning-based approach to
detect fraudulent transactions in banking data.
Data Collection
The dataset was sourced from Kaggle, containing real banking
transaction records.

Data Preprocessing
The data was analyzed to find any null value and to find the data type of
the features.

RESEARCH METHODOLOGY

Anomaly Detection Model Implementation
To detect fraudulent transactions, four machine learning algorithms were
applied:

-> K-Means Clustering
-> One-Class SVM
->Isolation Forest
->Local Outlier Factor (LOF)
Each algorithm was trained and tested on a subset of the dataset to
identify patterns of fraudulent activities.

Features used :
'Channel' , 'IP Address', 'DeviceID', 'Location', 'TransactionType',
'AccountID'
Feature selection and processing

Feature Selection: Only relevant columns like transaction amount,
transaction type, location, and account activity were selected.

KEY FINDINGS

Isolation forest algorithm

By using Isolation forest algorithm 126 anomalies were detected,
this algorithm uses multiple columns such as location, device id ,
transaction type , channel.
To maintain consistency across each model, all the algorithms use
the same columns

K means clustering

The accuracy percentage of the algorithms are calculated using
intersection method.
