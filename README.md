# AnomalyDetection-Capstone-Project
Overview

AnomaData is a project that focuses on automated anomaly detection for predictive maintenance. It aims to predict potential machinery failures before they occur, allowing for timely intervention. Using machine learning algorithms, the system can differentiate between normal and anomalous behavior in industrial operational data. The detection of anomalies enables proactive maintenance, reducing unexpected downtimes and maintenance costs.

Dataset Description

The dataset used for anomaly detection consists of sensor readings collected from industrial machinery over time. It includes both normal operational data and anomalies, which signify irregular or faulty machine behavior that could lead to breakdowns. The data comprises the following components:

Features: Continuous sensor data such as temperature, pressure, vibration, and more. Timestamps: Datetime values capturing when the sensor readings were recorded. Target (y): A binary variable indicating whether a data point is an anomaly (1) or not (0).

Project Goals

Anomaly Detection: Accurately detect anomalies in sensor data to identify machine failures in advance. Model Performance: Train and evaluate various machine learning models to identify the best-performing one. Real-Time Maintenance: Use the trained models to help implement predictive maintenance systems in industrial environments.

Machine Learning Models Four machine learning models were evaluated in this project:

Random Forest Classifier

Accuracy (after tuning): 99% Precision: 99% Recall: 99% F1-Score: 99% Best Performance: This model showed near-perfect results after hyperparameter tuning. It combines predictions from multiple decision trees, making it highly effective at detecting anomalies.

K-Nearest Neighbors (KNN)

Accuracy (after tuning): 97% Precision: 98% (non-anomalies), 96% (anomalies) Recall: 95% (non-anomalies), 99% (anomalies) F1-Score: 97% Explanation: KNN performed well by looking at similar data points to classify new data, making it effective at detecting patterns and anomalies.

Logistic Regression

Accuracy (after tuning): 86% Precision: 85% (non-anomalies), 88% (anomalies) Recall: 86% (non-anomalies), 85% (anomalies) F1-Score: 86% Explanation: Logistic Regression showed a balanced trade-off between precision and recall, making it a simple but reliable model.


Data Preprocessing: Clean and preprocess the dataset, including handling missing values, scaling features, and managing time-series data. Model Training: Train multiple machine learning models and apply resampling techniques such as SMOTE and RandomUnderSampler to handle class imbalance. Model Evaluation: Evaluate the models based on accuracy, precision, recall, F1-score, and confusion matrix, both before and after hyperparameter tuning. Best Model: The Random Forest Classifier was selected as the best model for anomaly detection, achieving the highest performance across all metrics.
