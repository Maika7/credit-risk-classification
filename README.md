# credit-risk-classification

# Module 12 Report

## Overview of the Analysis

In this project, we analyzed historical lending data to build a machine learning model capable of predicting the creditworthiness of borrowers. The data contains financial information about loans, and the primary goal was to predict the `loan_status`, where:

- `0` indicates a healthy loan.
- `1` indicates a high-risk loan.

We performed the following stages in the machine learning process:

1. **Data Preparation**: We read the data from a CSV file and separated the features (X) and labels (y).
2. **Data Splitting**: We split the data into training and testing datasets using an 80/20 split.
3. **Model Selection**: We used Logistic Regression, a binary classification algorithm, to create a predictive model.
4. **Evaluation**: We evaluated the model using a confusion matrix and a classification report to assess its performance in predicting both `0` and `1` labels.

---

## Results

### **Machine Learning Model 1: Logistic Regression**
- **Accuracy**: Achieved a high accuracy score, indicating the model correctly classified most loans.
- **Precision for Class `0` (Healthy Loans)**: High precision, meaning most loans predicted as healthy were actually healthy.
- **Precision for Class `1` (High-Risk Loans)**: Moderate precision, showing room for improvement in identifying high-risk loans.
- **Recall for Class `0` (Healthy Loans)**: High recall, indicating the model successfully identified most healthy loans.
- **Recall for Class `1` (High-Risk Loans)**: Moderate recall, showing the model missed some high-risk loans.

---

## Summary

The Logistic Regression model performs well overall, particularly in predicting healthy loans (`0`), with high accuracy and recall scores. However, the model’s precision and recall for high-risk loans (`1`) are moderate, suggesting some improvement is needed to better identify high-risk borrowers.

### **Recommendation**
We recommend using this model if predicting healthy loans (`0`) is a priority for the company. The model can reliably identify borrowers with low risk of default. However, if identifying high-risk loans (`1`) is more critical, further model optimization or alternative algorithms, such as Random Forest or Gradient Boosting, might be more effective.
