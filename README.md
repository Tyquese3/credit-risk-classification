Purpose of This Analysis

The goal of this analysis is to predict the loan status of borrowers using financial data, specifically loan size, interest rate, and borrower income. The classification model determines whether a loan is healthy or high risk, allowing financial institutions to make informed lending decisions.

Dataset Information

The dataset contains information about current customers' lending history, including:

Loan Size: The amount borrowed by the customer.

Interest Rate: The rate applied to the loan.

Borrower's Income: The income level of the borrower.

Using this financial data, a logistic regression model is trained to classify loan risk.

Machine Learning Workflow

The analysis follows several key stages in machine learning:

Read in the dataset containing customer lending history.

Split the data:

Separate the dataset into features (X) and target variable (y).

Further split the data into training and testing sets.

Train the Model:

Fit a Logistic Regression Classifier to the training data.

Make Predictions:

Use the trained model to predict loan risk status on the testing data.

Evaluate Performance:

Print a confusion matrix to assess prediction accuracy.

Generate a classification report to analyze precision, recall, and accuracy.

* Machine Learning Model 1:
    * Description of Model 1 Precision, and Recall scores.
Class 0 (Healthy Loans)
Precision (1.00): Out of all instances predicted as healthy loans (0), 100% were actually healthy.
Recall (0.99): The model correctly identified 99% of all actual healthy loans.

Class 1 (High-Risk Loans)
Precision (0.83): Out of all instances predicted as high-risk (1), 83% were truly high-risk.
Recall (0.95): The model correctly identified 95% of all actual high-risk loans.

*Summary
  The logistic regression model performs best, achieving 99% accuracy and this is the one i would recommend.
  It classifies healthy loans (Class 0) with near-perfect precision (1.00) and recall (0.99). For high-risk loans (Class 1), it has a high recall (0.95) but a lower
  precision (0.83), meaning some false positives occur. If the primary concern is avoiding high-risk loans, recall for Class 1 (0.95) is
  critical. The model successfully captures most high-risk borrowers, which helps prevent financial losses. In financial decision-making,
  predicting high-risk loans (Class 1) correctly is more important, as misclassifying them as healthy could result in loan defaults.
