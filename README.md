# Loan-Approval-Status-Prediction

This project aims to predict the approval status of loan applications based on applicant details such as income, credit history, and employment status. The model is trained on a dataset of past loan applications and their outcomes.

## Data
The data for this project is a sample of past loan applications and their outcomes. The data is in a CSV file called "loan_data.csv" and includes the following columns:

&#9658; Loan_ID: unique ID for each loan application

&#9658; Gender: gender of the applicant

&#9658; Married: marital status of the applicant

&#9658; Dependents: number of dependents of the applicant

&#9658; Education: education level of the applicant

&#9658; Self_Employed: whether the applicant is self-employed or not

&#9658; ApplicantIncome: annual income of the applicant

&#9658; CoapplicantIncome: annual income of the co-applicant

&#9658; LoanAmount: requested loan amount

&#9658; Loan_Amount_Term: term of the loan

&#9658; Credit_History: credit history of the applicant

&#9658; Property_Area: area of the property for which the loan is requested

&#9658; Loan_Status: outcome of the loan application (approved/rejected)


## Data Preprocessing
- In this project, null values are removed from the dataset so that the model can be trained on a complete set of data. This can be done by either dropping the rows with null values or filling them with a default value such as the mean or median of the column.

- Another important preprocessing step is encoding categorical variables. This way, the model can still make use of the ordinal relationship between categories, but the encoded variables are now numeric.

## Feature Engineering :
- Feature scaling is used to standardize the variables by transforming them to have a mean of 0 and a standard deviation of 1. 

- In this project we have used Standardscaler.This ensures that the test data is transformed in the same way as the training data and avoids any data leakage.

## Model Building :
- Model building is the process of using various machine learning algorithms to create a model that can accurately predict the outcome of new data.
- The three algorithms used in this project are 
&#9658; Logistic Regression,
&#9658;  Random Forest, 
&#9658;  Support Vector Machine. 
Pipeline and RandomizedSearchCV are two functions that were used to parallelize the hyperparameter tuning process. These functions help to find the best set of hyperparameters for a given model by automating the process of hyperparameter tuning and allow to test different combination of hyperparameters in parallel to find the best set of hyperparameters.

## Model Evaluation :
- Evaluating a model is an important step in the machine learning process as it helps to determine the performance of the model on unseen data. 
- In this project, the model is evaluated by passing a value from the dataset.

## GUI:
-  A GUI is built using tkinter library in Python in this project, which allows users to input attribute values and predict the status of loan approval. 

## Project Outcome:
&#9733; The outcome of this project is the ability to predict the approval status of loan applications based on applicant details such as income, credit history, and employment status. 

&#9733; Through the process of feature engineering, it was found that the 'Credit_History','Applicant Income','LoanAmount' features are the most important in determining the approval status of a loan application.

&#9733; A GUI (Graphical User Interface) was also built using the tkinter library in Python, which allows users to input attribute values and predict the status of loan approval.
