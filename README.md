# Credit Risk Classification

This project uses a logistic regression model tested on both the original and resampled datasets to create a comparative credit risk analysis report.

# Overview of the Analysis

This tool uses historical lending data to build a supervised ML model that predicts borrower creditworthiness based on various financial factors. It focuses on classifying loans as "healthy" or "high risk" using a Logistic Regression technique. The target variable is loan_status (0 or 1), and other data are features (X).

The ML process involves model creation, fitting, and utilization. Since healthy loans outnumber risky ones, this presents an imbalanced classification challenge.

To assess the model, dataset resampling was performed and tested with the initial model for efficiency.

# Results

- Machine Learning Model 1 - Logistic Regression:
    Accuracy: 0.9520479254722232
    Precision: 1.0 / 0.85
    Recall scores: 0.99 / 0.91

- Machine Learning Model 2 - Logistic Regression w/ ReSampled Data:
    Accuracy: 0.9936781215845847
    Precision: 1.0 / 0.84
    Recall scores: 0.99 / 0.99

# Summary
Both regression models did well in detecting healthy loans (precision = 1.0) but were less accurate with high-risk loans (0.85 vs. 0.84).

As for recall, the resampled model did better in detecting both healthy and high-risk loans (0.91 vs. 0.99).

In summary, the resampled data model showed an overall increase in accuracy for high-risk loan detection, with a higher balanced accuracy score (0.9937 vs. 0.9520), consistent with the classification report.

Given the imbalance in credit risk data, accurately predicting "high-risk loans" (0) is crucial. At this stage, I recommend exploring other machine learning classification techniques, such as "Support Vector Machines," "Decision Tree Based Algorithms," or "K-Nearest Neighbors," to further improve the prediction accuracy to 0.97 or higher.
