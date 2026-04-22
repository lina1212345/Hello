# LendingClub Loan Default Prediction
This project explores publicly available data from LendingClub.com. Lending Club connects people who need money (borrowers) with people who have money (investors). The goal is to create a model that predicts the probability of a borrower paying back their loan in full.

# Project Overview
Investors want to identify borrowers who have a high probability of paying them back. We use a dataset containing lending data from 2007-2010 to classify whether or not a borrower "not fully paid" their loan.

# Dataset Features

credit.policy: 1 if the customer meets credit underwriting criteria, 0 otherwise.

purpose: The purpose of the loan (e.g., debt_consolidation, credit_card, etc.).

int.rate: The interest rate of the loan.

installment: The monthly installments owed by the borrower.

log.annual.inc: Natural log of the self-reported annual income.

dti: Debt-to-income ratio.

fico: The FICO credit score of the borrower.

not.fully.paid: The target variable (1 if the loan was not paid back, 0 if it was).

# Workflow
1. Exploratory Data Analysis (EDA)

We visualized the data to find trends. Key insights included:

Borrowers with higher FICO scores are more likely to meet the credit policy.

The relationship between FICO scores and interest rates shows that riskier borrowers (lower FICO) are charged higher interest.

2. Categorical Features

Since the purpose column is categorical, we transformed it using Dummy Variables (one-hot encoding) so that the machine learning algorithms could process the information.

3. Model Building

We implemented two different tree-based algorithms:

Decision Tree Classifier: A single tree that splits data based on feature importance.

Random Forest Classifier: An ensemble method that uses a collection of decision trees to improve predictive accuracy and control over-fitting.

4. Evaluation

We evaluated the models using:

Confusion Matrix: To see the count of True Positives, True Negatives, False Positives, and False Negatives.

Classification Report: To analyze Precision, Recall, and F1-Score.

# Requirements
To run this notebook, you will need:

Python 3.x

Pandas

NumPy

Matplotlib

Seaborn

Scikit-learn

# Conclusion
While the Decision Tree is easier to interpret, the Random Forest generally performs better by reducing variance, though it may struggle with recall on the minority class (loans not paid) if the dataset is highly imbalanced.
