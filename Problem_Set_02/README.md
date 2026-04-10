# Bank Term Deposit Prediction

## Project Overview
This project is about predicting whether a customer will subscribe to a term deposit or not.  
I used the Bank Marketing dataset for this task. The main goal was to build a Logistic Regression model and check how well it can predict the result.

## Problem Statement
A banking institution wants to know if a customer will say "yes" or "no" to a term deposit offer based on their banking information and past behavior.

## Dataset
I used the **Bank Marketing Data Set**.

It contains customer details like:
- age
- job
- marital status
- education
- account balance
- contact type
- previous campaign result
- and other banking features

The target column is `y`, which shows:
- `yes` = customer subscribed
- `no` = customer did not subscribe

## Tools and Libraries
I used:
- Python
- Pandas
- NumPy
- Matplotlib → To plot the ROC curve
- Seaborn
- Scikit-learn

## Method Used
First, I loaded the dataset into Colab and checked the basic information about the data.

Then I did the following steps:

1. Loaded the CSV file
2. Checked missing values and data type
3. Converted categorical columns into numeric form
4. Split the dataset into input features and target column
5. Divided the data into training set and testing set
6. Scaled the features
7. Trained a Logistic Regression model
8. Predicted the test results
9. Evaluated the model using accuracy, confusion matrix, classification report, ROC curve, and AUC score

## Why Logistic Regression
Logistic Regression is a good choice for this problem because the output has only two classes:
- yes
- no

So it is a binary classification problem.

## Model Evaluation
To check the performance of the model, I used:

- Accuracy Score: 0.8878690699988941
- Confusion Matrix
- Classification Report
- ROC Curve
- AUC Score: 0.8700008253001049

These evaluation methods helped me understand how well the model is working.

## Result
The model was able to predict whether a customer will subscribe to a term deposit or not with good performance on the test data.

## Key Findings
- Overall Accuracy: The model demonstrated a high level of overall predictive accuracy.
- Class 0 Performance: The model shows significantly higher predictive power for Class 0 (no subscription) compared to other categories.
- Recall Disparity: The Recall for Class 1 (subscription: yes) is relatively low, indicating that the model struggled to identify all actual positive cases.
- Imbalanced Dataset: Because the dataset is imbalanced, accuracy is not a sufficient metric on its own. Consequently, the Confusion Matrix and Classification Report were analyzed to gain a more comprehensive understanding of performance.
- ROC-AUC Score: The ROC-AUC score confirms that the model’s performance is substantially better than a random guess.

