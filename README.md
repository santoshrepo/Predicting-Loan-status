# Predicting-Loan-status

# Introduction
Insurance stream is one of the largest use of data analytics method when compared to other fields. This domain gives the challenging part of working on the data from the insurance company. This is the classification dataset, which mainly depends on the type of strategies used, and variable that plays an important role in the target variable. It needs to be predicted about the loan eligibility process based on a few variables such as Gender, Marital Status, Education, Number of Dependents, Income, Loan Amount, Credit History and others. This dataset contains 614 rows and 13 columns. The dataset has one target variable, whereas 12 descriptive features. The target variable here is to check if an individual has got their loan sanction or not.

The target variable is of two types of levels;

- y is the person got their loan sanctioned
- n is the person failed to get their loan sanction.


This dataset contains 12 descriptive variables:

- Loan_ID: continuous
- Gender: male and female
- Dependents: 0, 1, 2 and 3+
- Education: Graduate and Not Graduate
- Self_Employed: yes and no
- ApplicantIncome: continuous
- Co-applicantIncome: continuous
- LoanAmount: continuous
- Loan_Amount_Term: continuous
- Credit_History: 0 and 1
- Property_Area: Rural, Urban and semiurban

# Methodology 

We build the following binary classifiers to predict the target feature:

* K-Nearest Neighbors (KNN),
* Decision trees (DT), and
* Naive Bayes (NB).

The cleaned dataset is transformed into Phase II from phase I. The transformation process includes encoding categorical descriptive features for target and descriptive respectively. All the observations are taken into consideration and the data is split into 70:30 ratio, where 70 refers to training sets and 30 is the test sets.

Random Forest method is used to check the best feature. 10,20 and all the features are given to select the best feature out of the dataset. To tune with hyperparameters, feature selection is pipelined with hyperparameter search. Then, the 5 fold is conducted with 2 repetitions.

From the training data, the best model is identified from KNN, NB, and DT respectively. 5-fold cross-validation is performed on the test data, following with the paired t-test to check if it is statistically significant or not. Moreover, all the classifiers are compared to check the scores and confusion matrices.

# How to run
* Download(Data and notebook) all the files in the repo
* Run the notebook file using Jupyter notebook
