# Practical 10: Scalable K-Means Clustering for Customer Segmentation using Apache Spark MLlib

## Challenges Faced

1. Loading and preprocessing customer transaction data and extracting meaningful behavioural features.
2. Creating customer-level features such as total spend, purchase frequency, average basket size, and recency.
3. Applying VectorAssembler, StandardScaler, and K-Means clustering using Apache Spark MLlib.
4. Evaluating clustering performance using WSSSE and the Elbow Method and interpreting the resulting customer segments.

## Solutions

1. Loaded the customer transaction dataset and grouped transactions by customer to generate the required behavioural features.
2. Used VectorAssembler and StandardScaler to create and normalize the feature vectors before clustering.
3. Applied Spark MLlib K-Means with different values of `k`, calculated WSSSE, and selected `k = 5` using Elbow Method analysis.
4. Generated customer clusters, summarized their behaviour, compared clustering methods, and interpreted the identified customer segments.
