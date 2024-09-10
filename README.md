# CancerClassification-ML
Prepared by Derick Cazares, Melissa Morales, Renee Perez, and Feven Surafel

## Overview
The objective of this project is to utilize the Wisconsin Breast Cancer Diagnostic Dataset for predictive analysis to improve early detection and diagnosis of breast cancer. By leveraging machine learning techniques, we seek to develop a predictive model that can classify tumor samples as malignant or benign based on various features extracted from cell nuclei.

## Results
**Machine Learning Linear Regression Model (XXX% Accuracy)**

* Class B (Benign Diagnosis)
    * Precision: 0.95, meaning that 95% of all predicted benign instances were correctly classified as benign.
    * Recall: 0.95, meaning that 95% of all actual benign cases were correctly identified.
 
* Class M (Malignant Diagnosis)
    * Precision: 0.93, meaning that 93% of all predicted malignant instances were correctly classified as malignant.
    * Recall: 0.93, meaning that 93% of all actual malignant cases were correctly identified.

## Analysis

### Purpose
The purpose of this analysis is to create a machine learning model capable of accurately classifying breast cancer tumors. This model can assist with early detection by analyzing features such as radius, texture, perimeter, and smoothness of cell nuclei.

### Data
The data used in this analysis comes from the Wisconsin Breast Cancer Diagnostic Dataset and includes:

569 samples
30 features representing characteristics of the tumor
Target labels: Benign (B) and Malignant (M)

Machine Learning Process
1. Data Preprocessing
The dataset was cleaned and split into training and testing sets using train_test_split. This ensures that the model is trained on one part of the data and evaluated on a separate part.
2. Model Training
A Logistic Regression model was selected for its effectiveness in binary classification tasks.
The model was trained using the training set and validated on the test set to assess its predictive power.
3. Evaluation Metrics
The model’s performance was measured using metrics such as precision, recall, F1-score, and accuracy.
A confusion matrix was generated to visualize the true positive, true negative, false positive, and false negative rates.
The ROC curve was used to examine the trade-off between sensitivity and specificity across different thresholds.
4. Correlation Analysis
A correlation matrix was computed to identify relationships between features and highlight any redundancies. Highly correlated features were noted for potential feature reduction.

## Summary
The Logistic Regression model performed well with an accuracy of 94%. It demonstrated high precision and recall for both benign and malignant tumor classifications, making it a strong candidate for this classification problem.


