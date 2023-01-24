# Loan-Approval-Status-Prediction

This project aims to predict the approval status of loan applications based on applicant details such as income, credit history, and employment status. The model is trained on a dataset of past loan applications and their outcomes.

## Data
The data for this project is a sample of past loan applications and their outcomes. The data is in a CSV file called "loan_data.csv" and includes the following columns:

Loan_ID: unique ID for each loan application
Gender: gender of the applicant
Married: marital status of the applicant
Dependents: number of dependents of the applicant
Education: education level of the applicant
Self_Employed: whether the applicant is self-employed or not
ApplicantIncome: annual income of the applicant
CoapplicantIncome: annual income of the co-applicant
LoanAmount: requested loan amount
Loan_Amount_Term: term of the loan
Credit_History: credit history of the applicant
Property_Area: area of the property for which the loan is requested
Loan_Status: outcome of the loan application (approved/rejected)


## Data Preprocessing
Data preprocessing is an important step in any machine learning project as it helps to prepare the data for modeling and improve the performance of the model.

One of the most common data preprocessing tasks is dealing with null or missing values. In this project, null values are removed from the dataset so that the model can be trained on a complete set of data. This can be done by either dropping the rows with null values or filling them with a default value such as the mean or median of the column.

Another important preprocessing step is encoding categorical variables. Categorical variables are non-numeric variables that can take on a limited number of values, such as gender, education level, or loan status. Since most machine learning models require numerical input, these variables need to be converted to numerical values.
Label encoding is a common method for encoding categorical variables. It assigns a unique integer value to each category. This way, the model can still make use of the ordinal relationship between categories, but the encoded variables are now numeric.

# Feature Engineering :
In feature engineering, we use various techniques to extract useful information from the raw data and create new features that can improve the performance of the model.
One such technique is feature scaling, which is used to standardize the variables by transforming them to have a mean of 0 and a standard deviation of 1. This is important because many machine learning models, such as linear and logistic regression, are sensitive to the scale of the input variables.

In this project we have used Standardscaler.StandardScaler is a popular tool in Python's scikit-learn library that can be used to standardize the variables. It works by fitting the scaler to the training data and then transforming both the training and test data using the same scaler. This ensures that the test data is transformed in the same way as the training data and avoids any data leakage.

# Model Building :
Model building is the process of using various machine learning algorithms to create a model that can accurately predict the outcome of new data. The three algorithms used in this project are Logistic Regression, Random Forest, and Support Vector Machine. Pipeline and RandomizedSearchCV are two functions that were used to parallelize the hyperparameter tuning process. These functions help to find the best set of hyperparameters for a given model by automating the process of hyperparameter tuning and allow to test different combination of hyperparameters in parallel to find the best set of hyperparameters.

# Model Evaluation :
Evaluating a model is an important step in the machine learning process as it helps to determine the performance of the model on unseen data. In this project, the model is evaluated by passing a value from the dataset.

# GUI:
 A GUI is built using tkinter library in Python in this project, which allows users to input attribute values and predict the status of loan approval. Tkinter is a built-in library in Python for creating graphical user interfaces and it provides a set of widgets such as buttons, labels, and text boxes. Building a GUI can make the model more accessible and user-friendly. The GUI in this project allows users to input the attribute values easily and quickly and the model makes the predictions in real-time, saving time and effort compared to manually inputting the values into the model and running it on the command line.


# Project Outcome:
The outcome of this project is the ability to predict the approval status of loan applications based on applicant details such as income, credit history, and employment status. Through the process of feature engineering, it was found that the 'Credit_History','Applicant Income','LoanAmount' features are the most important in determining the approval status of a loan application.

In the feature engineering process, various techniques were used to extract useful information from the raw data and create new features that can improve the performance of the model. This process helped in identifying the most important features that have a strong impact on the target variable which is loan approval status.

A GUI (Graphical User Interface) was also built using the tkinter library in Python, which allows users to input attribute values and predict the status of loan approval.
