# **Supervised Learning**

# Metaverse Financial Transactions

## How to run

Please open the `src/financial_transactions.ipynb` file in Jupyter Notebook (or the IDE of your choice) and run the cells.
All the compilation instructions are in the notebook, as well as comments made throughout the evolution of the project.

---

This project was made by:

| Name | UP |
|-|-|
| Ana Carolina Coutinho | up202108685 |
| José Costa | upxxxx |
| Afonso Poças | upxxxx |
|---|---|


Introduction
------------

This project focuses on detecting anomalies, performing fraud analysis, and assessing risks in financial transactions within the Metaverse using various machine learning algorithms. The goal is to categorize transactions into different risk levels based on their attributes, such as transaction type, user behavior, and transaction amount.

Dataset
-------

The Metaverse Financial Transactions Dataset comprises 78,600 blockchain-based transactions, offering detailed attributes such as timestamps, addresses, transaction types, and risk scores. This dataset supports research in fraud detection, risk assessment, and user behavior analysis in virtual environments.

Problem Statement
-----------------

We aim to develop predictive models for anomaly detection and risk assessment in Metaverse financial transactions. This is a multivariate classification problem, where transactions need to be categorized into different risk levels (high, moderate, or low risk).

Solution
--------

### Data Understanding and Preprocessing

Data Exploration

-   Attributes include timestamp, hour of day, sending and receiving addresses, amount, transaction type, location region, IP prefix, login frequency, session duration, purchase pattern, age group, risk score, and anomaly level.

Data Cleaning

1.  Handling Missing Values: Imputation or removal to ensure data integrity.
2.  Data Formatting: Convert categorical variables into numerical formats using one-hot encoding.
3.  Normalization: Standardize the scale of continuous variables to improve model performance.

Feature Engineering

1.  Time-Based Features: Extract additional features like day of the week or part of the day.
2.  Behavioral Features: Aggregate features summarizing user behaviors.
3.  Risk Indicators: Develop custom risk indicators based on combinations of different attributes.

### Model Development

Algorithm Selection We evaluated several machine learning algorithms for their effectiveness in anomaly detection:

1.  Random Forest: Ensemble method for robust anomaly detection.
2.  Gradient Boosting Machines (GBM): Effective for imbalanced datasets.
3.  Support Vector Machines (SVM): Optimal hyperplane classification.
4.  Neural Networks (MLP): Captures complex patterns.
5.  k-Nearest Neighbors (k-NN): Simple, instance-based learning.

Model Training

1.  Data Splitting: Split dataset into training and test sets for robust evaluation.
2.  Hyperparameter Tuning: Optimize model parameters using grid search or random search.
3.  Cross-Validation: Implement k-fold cross-validation to validate model performance and prevent overfitting.

Model Evaluation

1.  Performance Metrics: Use precision, recall, F1-score, and ROC-AUC to evaluate models.
2.  Threshold Selection: Determine optimal threshold for classifying transactions as anomalies based on precision-recall trade-off.

### Conclusion

The Random Forest model was chosen for its superior performance in handling complex and varied data typical of the Metaverse environment. This project has been a valuable learning experience, providing practical insights into applying machine learning techniques to real-world challenges. We have established a robust model that enhances the security of financial transactions within virtual economies, laying a solid foundation for future research and applications.
