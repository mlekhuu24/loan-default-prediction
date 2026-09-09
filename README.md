# loan-default-prediction
Loan Default Prediction is a machine learning project that predicts whether a loan applicant is likely to repay a loan or potentially default. It uses factors such as income, loan amount, credit score, employment status, existing loans, and debt-to-income ratio. The project uses Logistic Regression for binary classification.
# Loan Default Prediction Using Machine Learning

## Project Overview

Loan Default Prediction is a machine learning project developed using Python to predict whether a loan applicant is likely to repay a loan or potentially default.

The project analyzes applicant information such as age, annual income, loan amount, credit score, employment status, loan term, existing loans, debt-to-income ratio, and home ownership.

A Logistic Regression model is used to classify loan applications into two categories: likely repayment and potential default.

This project is intended for educational and academic purposes.

## Objectives

* Analyze loan application data.
* Identify factors related to loan repayment and default.
* Preprocess the loan application dataset.
* Train a machine learning classification model.
* Predict potential loan defaults.
* Calculate the probability of default.
* Evaluate the performance of the model.
* Identify important factors related to loan default.
* Visualize loan and default patterns.

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn

## Machine Learning Algorithm

### Logistic Regression

The project uses Logistic Regression for binary classification.

The model predicts two possible outcomes:

* `0` - Likely Repayment
* `1` - Potential Default

Logistic Regression is a supervised machine learning algorithm commonly used for binary classification problems.

## Dataset

The project uses the following dataset:

`loan_default.csv`

### Dataset Features

| Feature              | Description                                   |
| -------------------- | --------------------------------------------- |
| applicant_id         | Unique identification number of the applicant |
| age                  | Age of the applicant                          |
| annual_income        | Annual income of the applicant                |
| loan_amount          | Amount of loan requested                      |
| credit_score         | Credit score of the applicant                 |
| employment_status    | Employment status of the applicant            |
| loan_term_months     | Loan repayment period in months               |
| existing_loans       | Number of existing loans                      |
| debt_to_income_ratio | Ratio of debt to income                       |
| home_ownership       | Home ownership status                         |
| loan_default         | Target variable indicating loan default       |

### Target Variable

`loan_default`

The target variable represents whether the applicant is likely to repay or potentially default.

## Project Workflow

The project follows these steps:

1. Load the loan dataset.
2. Display the first five records.
3. Check the dataset shape.
4. Check for missing values.
5. Separate input features and target variable.
6. Remove the applicant ID from the input features.
7. Handle missing numerical values.
8. Handle missing categorical values.
9. Standardize numerical features.
10. Encode categorical features.
11. Split the dataset into training and testing data.
12. Train the Logistic Regression model.
13. Generate predictions.
14. Calculate model accuracy.
15. Generate a classification report.
16. Generate a confusion matrix.
17. Predict a new loan applicant.
18. Calculate default probability.
19. Analyze important model factors.
20. Generate visualizations.

## Data Preprocessing

The project uses different preprocessing methods for numerical and categorical features.

### Numerical Features

The numerical features include:

* Age
* Annual income
* Loan amount
* Credit score
* Loan term
* Existing loans
* Debt-to-income ratio

Missing numerical values are replaced using median values.

The numerical features are standardized using `StandardScaler`.

### Categorical Features

The categorical features include:

* Employment status
* Home ownership

Missing categorical values are replaced using the most frequent value.

Categorical features are converted into numerical values using One-Hot Encoding.

## Train-Test Split

The dataset is divided into:

* 80% Training Data
* 20% Testing Data

Stratified splitting is used to maintain the distribution of the target classes in the training and testing datasets.

## Model Evaluation

The model is evaluated using:

### Accuracy

Accuracy represents the percentage of correctly classified loan applications.

### Classification Report

The classification report provides:

* Precision
* Recall
* F1-score
* Support

These metrics provide detailed information about the model's classification performance.

### Confusion Matrix

The confusion matrix shows the number of correctly and incorrectly classified applications for each category.

## New Loan Applicant Prediction

The project demonstrates how the trained model can predict the result for a new loan applicant.

The example applicant contains information such as:

* Age
* Annual income
* Loan amount
* Credit score
* Employment status
* Loan term
* Existing loans
* Debt-to-income ratio
* Home ownership

The model predicts whether the applicant is likely to repay or potentially default and also calculates the estimated default probability.

## Feature Importance

The project analyzes the Logistic Regression coefficients to identify the factors that have the greatest influence on loan default prediction.

The features are ranked based on their absolute coefficient values.

This helps identify which applicant characteristics have a stronger relationship with the model's predictions.

## Data Visualization

The project generates two visualizations.

### 1. Credit Score and Loan Amount vs Default

This scatter plot shows the relationship between credit score and loan amount while indicating the loan default category.

Output file:

`credit_score_vs_loan_amount.png`

### 2. Loan Default Rate by Employment Status

This bar chart displays the default rate for different employment statuses.

Output file:

`default_by_employment.png`

## Project Structure

```text
Loan_Default_Prediction/
│
├── loan_default_prediction.py
├── loan_default.csv
├── requirements.txt
└── README.md
```

The visualization files are generated automatically when the program is executed.

## Installation

Make sure Python is installed on your computer.

Install the required libraries using:

```bash
pip install -r requirements.txt
```

Required libraries:

```text
pandas
numpy
matplotlib
scikit-learn
```

## How to Run

Open Command Prompt or Terminal in the project folder.

Run:

```bash
python loan_default_prediction.py
```

The program will:

* Load the loan dataset.
* Display basic dataset information.
* Check for missing values.
* Preprocess the data.
* Train the Logistic Regression model.
* Calculate model accuracy.
* Display the classification report.
* Display the confusion matrix.
* Predict a new loan applicant.
* Calculate default probability.
* Display important model factors.
* Generate visualization graphs.

## Applications

Loan default prediction can be useful for:

* Financial data analysis
* Risk assessment research
* Loan application analysis
* Credit risk management
* Banking analytics
* Financial machine learning applications

## Limitations

* The dataset included in this project is synthetic.
* The project is intended for educational purposes.
* Real-world loan decisions involve many additional factors.
* Model predictions depend on the quality and quantity of the training data.
* The model should not be used as the sole basis for actual lending decisions.

## Future Enhancements

The project can be improved by:

* Using larger real-world datasets.
* Comparing multiple classification algorithms.
* Implementing Random Forest and Gradient Boosting.
* Using Support Vector Machines.
* Performing feature selection.
* Applying cross-validation.
* Tuning model hyperparameters.
* Developing a web-based loan prediction application.
* Creating an interactive risk analysis dashboard.
* Deploying the model for real-time prediction.

## Project Information

**Project Name:** Loan Default Prediction

**Domain:** Machine Learning and Financial Analytics

**Programming Language:** Python

**Machine Learning Type:** Supervised Learning

**Problem Type:** Binary Classification

**Algorithm:** Logistic Regression

**Target Variable:** Loan Default

## Dataset Note

The dataset included in this project is synthetic and intended for educational and classroom machine learning practice. It does not contain real applicant information.

## Important Note

This project is intended for educational purposes. Model predictions should not be used as the sole basis for real-world lending, credit, or financial decisions.
