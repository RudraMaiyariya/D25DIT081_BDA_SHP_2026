Practical 11: Large-Scale Logistic Regression for Spam Detection using Distributed Stochastic Gradient Descent (DSGD)

## Challenges Faced

1. Loading and processing a large-scale SMS spam dataset containing 5 million records using PySpark.
2. Performing text preprocessing using tokenization, stop-word removal, TF-IDF feature extraction, and conversion into machine-learning features.
3. Implementing Logistic Regression with distributed stochastic gradient descent and tuning parameters such as regParam, maxIter, and elasticNetParam.
4. Evaluating the spam detection model using Accuracy, Precision, Recall, F1-Score, and ROC-AUC and comparing full-batch and mini-batch training performance.

## Solutions

1. Created and loaded a 5-million-record SMS spam dataset into a PySpark DataFrame and validated its schema, record count, labels, and missing values.
2. Used RegexTokenizer, StopWordsRemover, HashingTF, and IDF to convert SMS messages into numerical TF-IDF feature vectors.
3. Used Spark ML Logistic Regression for hyperparameter tuning and Spark MLlib LogisticRegressionWithSGD for full-batch and mini-batch distributed stochastic gradient descent.
4. Calculated Accuracy, Precision, Recall, F1-Score, and ROC-AUC and generated comparisons of training time and accuracy for different dataset sizes.
