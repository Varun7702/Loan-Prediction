# Loan-Prediction Project
This project aims to predict whether a loan applicant will be granted a loan or not, based on various features like applicant details, loan amount, credit history, etc. The notebook includes steps for data preprocessing, feature selection, model training, and performance evaluation.

## Project Overview
The goal of this project is to build a machine learning model that predicts whether a loan will be approved. This is a classification problem where the target variable is binary (loan approved or not).

## Dataset
The dataset contains the following features:

- **Applicant Details**: Gender, Married, Dependents, Education, Self_Employed, etc.
- **Loan Information**: Loan Amount, Loan Term, Credit History, etc.
- **Target Variable**: Loan_Status (1 = approved, 0 = not approved)

## Steps Involved

### 1. Data Preprocessing
- Handling missing values
- Encoding categorical features using label encoding and one-hot encoding
- Feature scaling for numerical variables

### 2. Feature Engineering
- Transformation and selection of relevant features based on correlation and domain knowledge.

### 3. Model Training
The following models were explored for prediction:

- Logistic Regression
- Random Forest
- Decision Tree

The models were fine-tuned using `RandomizedSearchCV` for hyperparameter optimization.

### 4. Model Evaluation
The models were evaluated using various metrics:

- **Accuracy**: Measures the overall correctness of the model.
- **Precision**: Measures the proportion of positive predictions that were actually correct.
- **Recall**: Measures the proportion of actual positives that were predicted correctly.
- **F1-Score**: Harmonic mean of precision and recall to provide a balanced metric.

Best model performance:

- **Accuracy**: 84.86%
- **Precision**: 82.78%
- **Recall**: 98.42%

## Dependencies
- Python 3.11
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
