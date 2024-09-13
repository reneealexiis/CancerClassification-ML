# Cancer Classification with Machine Learning

Prepared by: Derick Cazares, Melissa Morales, Renee Perez, and Feven Surafel

## Overview
The objective of this project is to utilize the Wisconsin Breast Cancer Diagnostic Dataset for predictive analysis to improve early detection and diagnosis of breast cancer. By leveraging machine learning techniques, we seek to develop a predictive model that can classify tumor samples as malignant or benign based on various features extracted from cell nuclei.

## Purpose
The goal is to create a machine learning model that accurately classifies breast cancer tumors. The model evaluates features such as radius, texture, perimeter, and smoothness of cell nuclei to assist with early detection.

## Data

**Source:**
The dataset used for this analysis is the [Wisconsin Breast Cancer Diagnostic Dataset](https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data?resource=download), which includes:

- **569 samples**: 357 benign, 212 malignant
- **30 features** representing tumor characteristics
- **Target labels**: Benign (B) and Malignant (M)

## Machine Learning Process
1. Retrieve the dataset from Spark and launch the notebook in Google Colab.
2. Split the data into training and testing sets.
3. Train a logistic regression model on the training data (X_train and y_train).
4. Generate and save predictions for the testing data (X_test).
5. Evaluate performance using a confusion matrix and classification report.
6. Optimize and refine the model through iterative improvements.

## Results

**Random Forest Model: 95% Accuracy**

- **Class B (Benign)**
  - Precision: 0.96 (96% of predicted benign cases were correctly classified)
  - Recall: 0.99 (99% of actual benign cases were correctly identified)

- **Class M (Malignant)**
  - Precision: 0.98 (98% of predicted malignant cases were correctly classified)
  - Recall: 0.93 (93% of actual malignant cases were correctly identified)

**Logistic Regression Model with Interaction Terms: 97% Accuracy**

Interaction terms enhance the model by capturing the combined effect of feature pairs:

- **Class B (Benign)**
  - Precision: 0.96 (96% of predicted benign cases were correctly classified)
  - Recall: 1.00 (100% of actual benign cases were correctly identified)

- **Class M (Malignant)**
  - Precision: 1.00 (100% of predicted malignant cases were correctly classified)
  - Recall: 0.92 (92% of actual malignant cases were correctly identified)

## Analysis
Both models performed well, with the Random Forest achieving 95% accuracy. However, the Logistic Regression model with interaction terms showed superior performance, achieving 97% accuracy. The high precision and recall for both classes indicate the model’s robustness in classifying tumors accurately.

## Summary and Next Steps
- This project developed a machine learning model for classifying breast cancer biopsy samples as benign or malignant, using the Wisconsin Breast Cancer Diagnostic Dataset.
- The Random Forest model outperformed the logistic regression model in recall for malignant cases, a crucial factor when addressing high-risk patients
- **Our team recommends the Logistic Regression model, enhanced with interaction terms, as it achieved a 97% accuracy, reflecting a +1% improvement in performance**
- Moving forward, next steps include further optimizing the model by exploring additional feature interactions and employing other advanced machine learning techniques.
- Additionally, validating the model with external datasets and integrating it into clinical workflows could enhance its practical utility for early breast cancer detection.

## Instructions for Final Work
Two notebooks are available in the repository for running in Google Colab:
- **"Breast_Cancer_Logistic_Regression_Model-Colab.ipynb"**
- **"Breast_Cancer_Random_Forest_Model-Colab.ipynb"**

Presentation is available to view bin the repository: 
- **Breast_Cancer_ML_Powerpoint_Final.pdf**
