# Customer-Churn-Analysis

## Overview
This project aims to develop a machine learning model to predict customer churn, helping businesses identify at-risk customers and enhance retention strategies. The model leverages various data points related to customer behavior and demographics to make accurate predictions.

## Table of Contents
- introduction
- data-overview
- data-preprocessing
- feature-engineering
- model-training
- model-evaluation
- model-interpretation
- conclusion

## Introduction
Customer churn prediction is a crucial aspect for businesses aiming to maintain a loyal customer base. By predicting which customers are likely to churn, companies can take proactive measures to retain them. This project uses machine learning algorithms to build a predictive model for customer churn.

## Data Overview
The dataset includes customer demographics, services subscribed to, and their usage patterns. Key features include:
- Demographics: Gender, Senior Citizen, Partner, Dependents
- Services: Phone Service, Multiple Lines, Internet Service, Online Security, Online Backup, Device Protection, Tech Support, Streaming TV, Streaming Movies
- Account Information: Contract Type, Paperless Billing, Payment Method, Monthly Charges, Total Charges, Tenure
- Support Tickets: Number of administrative and technical tickets

## Data Preprocessing
### Steps Taken:
1. Dropping Irrelevant Columns: Removed the 'customerID' column.
2. Handling Data Types: Converted 'TotalCharges' from object to numeric.
3. Handling Missing Values: Addressed any missing data points appropriately.
4. Encoding Categorical Variables: Applied one-hot encoding to convert categorical variables into numerical values.
5. Feature Scaling: Normalized features to ensure uniform scale.

## Feature Engineering
### New Features Created:
- Interaction Terms: Combined certain features to capture interactions.
- Aggregated Metrics: Created new features like average tenure and average monthly charges.

## Model Training
### Algorithms Used:
- Logistic Regression: For its simplicity and interpretability.
- Decision Trees: To capture non-linear relationships.
- Random Forests: To reduce overfitting and improve accuracy.

### Training Process:
- Split the dataset into a 70% training set and a 30% testing set.
- Trained the models on the training data.
- Tuned hyperparameters using cross-validation for optimal performance.

## Model Evaluation
### Performance Metrics:
- Accuracy: Overall correctness of the model.
- Precision: True positive rate among predicted positives.
- Recall: True positive rate among actual positives.
- F1-Score: Harmonic mean of precision and recall.
- ROC-AUC: Area under the ROC curve to evaluate performance.

### Validation Techniques:
- K-Fold Cross-Validation: Ensured model generalization across different subsets of data.

### Confusion Matrix:
- Visualized true positives, false positives, true negatives, and false negatives.

## Model Interpretation
### Key Findings:
- Top Features: Monthly Charges, Tenure, Contract Type, Payment Method.
- High Churn Risk: Customers with month-to-month contracts and higher monthly charges are more likely to churn.

### Visualizations:
- Feature Importance Plot: Highlighted the significance of each feature.
- ROC Curve: Showed the trade-off between true positive rate and false positive rate.
- Confusion Matrix: Illustrated model performance.

## Conclusion
This project demonstrates the power of machine learning in predicting customer churn. By identifying key drivers of churn, businesses can implement targeted retention strategies to minimize churn rates and maintain a loyal customer base. The model's deployment further ensures that predictions are actionable and integrated into daily operations.

## Author
Dhrumil Prajapati
