# Project Overview
This project demonstrates the use of the K-Nearest Neighbors (KNN) algorithm to classify data points based on multiple features. The goal is to predict the target class using a supervised machine learning approach.
The dataset is first standardized, then split into training and testing sets, and finally used to train and evaluate a KNN model.
# Dataset Description
The dataset contains several numerical features and a target variable:
Features: Multiple numerical attributes used for prediction
Target Column: TARGET CLASS (binary classification: 0 or 1)
# Steps Performed
1. Import Libraries
We used:
pandas
numpy
matplotlib
seaborn
sklearn
2. Data Exploration
Loaded dataset using pandas
Checked structure and summary using .info() and .head()
Visualized relationships using pairplot
3. Feature Scaling
Since KNN is distance-based, we standardized features using:
StandardScaler
Transformed data into a scaled feature set
4. Train-Test Split
Split data into:
70% training data
30% testing data
5. Model Training
Used KNeighborsClassifier
Started with K = 1
6. Model Evaluation
Predicted test data
Evaluated using:
Confusion Matrix
Classification Report (Precision, Recall, F1-score)
7. Choosing Best K Value
Tested K values from 1 to 40
Plotted Error Rate vs K Value
Selected optimal K based on lowest error rate
8. Final Model
Re-trained model using best K value (e.g. K = 30)
Achieved improved accuracy
# Results
The model achieved good classification performance
Accuracy improved after selecting optimal K
Feature scaling significantly improved performance
# Key Learning Outcomes
Understanding of KNN algorithm
Importance of feature scaling
Model evaluation techniques
Hyperparameter tuning (choosing K)
