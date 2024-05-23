# Loan_Eligibility_Prediction
This repository contains a data analytics project focused on predicting loan eligibility using various machine learning techniques. It includes data preprocessing, exploratory data analysis, model building, and evaluation to determine the factors influencing loan approval.

![image](https://github.com/lekshmiij/Loan_Eligibility_Prediction/assets/141242851/bb31ac90-6a0f-4377-a865-68e7abb63cfd)
This project involves a comprehensive process to predict loan eligibility using machine learning techniques. Here is an overview of the key steps:

### Data Loading and Initial Exploration:
The training dataset is loaded using pandas.
Basic data exploration is conducted with .head(), .shape(), .info(), and .describe() to understand the structure, size, and statistical properties of the data.
Crosstabs and visualizations (e.g., boxplots, histograms) are created to explore the relationship between features and loan status, and to identify outliers and data distribution issues.

### Handling Missing Values:

Missing values are identified using .isnull().sum().
Missing categorical values (Gender, Married, Dependents, Self_Employed, Credit_History, and Loan_Amount_Term) are filled with the mode.
Missing numerical values (LoanAmount and its log transformation) are filled with the mean.

### Feature Engineering and Data Transformation:

A new feature Total_Income (sum of ApplicantIncome and CoapplicantIncome) is created, and its log transformation (Total_Income_log) is added to the dataset.
Normalization is performed on LoanAmount using a log transformation to handle skewed data.

### Data Preparation for Modeling:

Independent variables (X) and the dependent variable (y) are selected.
The dataset is split into training and testing sets using train_test_split.
Categorical features are encoded using LabelEncoder to convert them into numerical form.

### Data Scaling:

Features are scaled using StandardScaler to ensure that all variables contribute equally to the model performance.

### Model Training and Evaluation:

A Decision Tree Classifier is trained on the scaled training data. The model's predictions are evaluated, but due to low accuracy, an alternative model is considered.
A Gaussian Naive Bayes Classifier is trained and evaluated, showing the prediction accuracy.
Application to Test Data:

The test dataset is processed similarly by filling missing values, creating and transforming features, and scaling the data.
The trained Naive Bayes model is used to predict the loan eligibility on the test dataset.

### Summary of Model Performance:

The accuracy of both models (Decision Tree and Naive Bayes) is calculated and compared.
This process involves thorough data preprocessing, feature engineering, handling of categorical variables, data scaling, and model training and evaluation to predict loan eligibility effectively.






