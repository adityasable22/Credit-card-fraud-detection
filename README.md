# Credit-card-fraud-detection
Project Overview
The Credit Card Fraud Detection System aims to detect and prevent fraudulent credit card transactions in real-time. This machine learning model leverages a deep neural network trained on anonymized transaction data to distinguish between legitimate and fraudulent activities, providing a scalable, automated solution to enhance financial security.

Motivation
In the era of digital payments, the rise of credit card fraud poses significant risks to financial institutions and individuals. Existing rule-based methods often fail to adapt to evolving fraud tactics. This project addresses these limitations by employing deep learning to recognize fraud patterns, reduce false positives, and maintain customer trust.

Key Features
Real-time Fraud Detection: Classifies transactions as they occur, minimizing response time.
High Accuracy: A neural network model that effectively balances fraud detection with minimizing disruptions to legitimate users.
Scalability: Capable of handling large transaction volumes, adapting to various financial systems.
Continuous Learning: Model updates to reflect new transaction behaviors and emerging fraud trends.
Dataset
The dataset contains anonymized credit card transaction data, including:
Time: Elapsed time since the first transaction.
V1 to V28: Principal Component Analysis (PCA) features that anonymize sensitive information.
Amount: Transaction amount, used as a feature.
Class: Target variable where 1 indicates fraud and 0 indicates a legitimate transaction.
Data Preprocessing
Cleaning: Removed irrelevant columns (e.g., Time) and verified there were no missing values.
Class Imbalance Handling: Applied Synthetic Minority Over-sampling Technique (SMOTE) due to the low number of fraudulent cases.
Feature Scaling: Standardized features for optimal neural network performance.
Model Architecture
The model is a deep neural network designed to capture complex fraud patterns with the following layers:

Input Layer: Receives anonymized transaction data.
Hidden Layers: Three dense layers with 64, 32, and 16 neurons, interspersed with dropout layers to reduce overfitting.
Output Layer: A single neuron with a sigmoid activation function to classify transactions as fraudulent or not.
Training & Evaluation
Training: The model is trained with binary cross-entropy loss and the Adam optimizer, balancing efficiency with adaptability.
Evaluation: Model performance is measured using precision, recall, F1 score, and accuracy to account for the class imbalance.
Results
The model demonstrates high performance, achieving significant accuracy, and minimizing both false positives and false negatives, crucial for operational efficiency and customer satisfaction.

Future Enhancements
Adaptability: Extend the model to detect other types of financial fraud, such as insurance fraud or money laundering.
Scalability: Integrate the model within real-time transaction systems in banking and e-commerce sectors.
Usage
This repository includes scripts for preprocessing, model training, and evaluation. Clone this repository, install the necessary dependencies, and follow the setup instructions to test the model on new datasets.

