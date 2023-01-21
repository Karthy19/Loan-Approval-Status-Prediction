# Loan-Approval-Status-Prediction

Prediction of loan approval status based on applicant details.


# Data Preprocessing
In  Data Preprocessing null values are removed and label encoding is performed for categorial attributs.

# Feature Engineering :
in FE part, we used standardscaler technique to standardise the variables.

# Model Building :
in this project of model building we used 10 different algorithms 1), Logistic Regression 2), Random Forest 3), Support Vector Machine.
pipeling and RandomizedSearchCV functions are used for parallising hyperparameter tuning.

# Model Evaluation :
Model is evaluated by passing a value from the dataset.

# GUI:
A GUI is build using tkinter that gets attributes values from users and predicts the status for loan approval.


# Project Outcome:
We can find out that 'Credit_History','Applicant Income','LoanAmount' feature are most important. 
So, feature engineering helped us in predicting our target variable and  a GUI was Build.
