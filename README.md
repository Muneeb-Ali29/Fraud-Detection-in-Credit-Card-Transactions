# **Credit Card Fraud Detection in Transactions**

![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)

## **Table of Contents**
- [Project Overview](#project-overview)
- [Data Understanding and Preprocessing](#data-understanding-and-preprocessing)
- [Feature Engineering](#feature-engineering)
- [Model Building and Evaluation](#model-building-and-evaluation)
- [Fraud Detection System Design](#fraud-detection-system-design)
- [Results and Visualizations](#results-and-visualizations)
- [How to Use](#how-to-use)
- [Contributing](#contributing)
- [License](#license)

## **Project Overview**
This project aims to detect fraudulent credit card transactions using various machine learning algorithms. It involves data preprocessing, feature engineering, model building, and evaluation to develop a robust fraud detection system.

## **Data Understanding and Preprocessing**
- **Dataset:** The dataset contains 363 records with 9 features: `Transaction ID`, `Customer ID`, `Transaction Date`, `Transaction Amount`, `Merchant`, `Location`, `Transaction Type`, `Card Type`, and `Is Fraudulent`.
- **Preprocessing Steps:**
  - Handled missing data (none in the dataset).
  - Encoded categorical variables using LabelEncoder.
  - Standardized the `Transaction Date` column.
  - Verified data balance, with a balanced class ratio.

## **Feature Engineering**
- Created new features such as:
  - `Transaction Frequency`: Frequency of transactions by a customer.
  - `Average Transaction Amount`: Average amount of transactions by a customer.
  - `Transaction Hour`: Time of day the transaction occurred.
  - `Type_Amount Interaction`: Interaction between transaction type and amount.
- Analyzed feature correlations using a heatmap.

## **Model Building and Evaluation**
- **Algorithms Used:**
  - Logistic Regression
  - Random Forest Classifier
  - Gradient Boosting Classifier
- **Evaluation Metrics:**
  - Accuracy, Precision, Recall, F1-Score
  - AUC-ROC for imbalanced datasets
- **Results:**
  - Tuned Random Forest model using Grid Search with an AUC-ROC of 0.634.

## **Fraud Detection System Design**
Proposed a real-time fraud detection system integrating machine learning models into the financial institution's transaction processing pipeline. Suggestions for continuous learning and adaptation to evolving fraud patterns are included.

## **Results and Visualizations**
- **Data Distribution:** Visualized class balance and transaction amount distribution.
- **Model Performance:** Confusion matrices and feature importance charts.
- **AUC-ROC Curves:** Comparison of models based on AUC-ROC scores.
