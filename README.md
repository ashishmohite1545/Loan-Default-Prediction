# Loan-Default-Prediction

1.	Business Context:

The challenge is to recognize Loan default applicants so that the Banks does not give loans to bad loan credit applicants. Main challenges involved in loan default detection are 
• Enormous Data: The major problem is lot of data is processed every day and the model build must be fast enough so that Bank doesn’t give out loan to defaulter applicants. 

• Imbalanced Data: As sometimes the banks miss out to give loans to low credit score applicants who have never defaulted on their loan payments.

 • Data availability: As per government and banks policy and due to high competition the banks doesn’t share the customer data.


2.	Problem Statement:

The aim of this project is minimize the Financial Institutions non performing assets by predicting the patterns of customers who are likely to default on loan.

3.	Solution Developed:
First, the data cleaning is performed as there were null values present for the categorical variables such as Gender", "Married", "Self_Employed so the null values are replaced by 
Mode and for numerical variables such as  LoanAmount, Loan_Amount_Term, Credit_History null values are replaced by mean. In addition to that bar chart are ploted to have an idea about the column specific approval or disapproval of loan. 

After plotting the bar chart it is found that:
1.	Males have higher chance of getting their loan approved and also higher chances of getting it disapproved.
2.	Those who are married have high chances of getting loan.
3.	Those who are Graduated have high chances of getting loan.
4.	Those who are not self employed have high chances of getting loan.
After that created few machine learning model that can predict if the loan applicant will default on loan or not. And the final model is a Decision Tree as it was having the highest accuracy among the other models that were created. 
4.	Improvements to the solution:
The base model for the project was a GaussianNB and it was having less accuracy compared to other model. After GaussianNB few more models were created such as Support Vector Machine with GridSearchCV, DecisionTree, RandomForestClassifier, XGBclassier. But DecisionTree was getting the highest accuracy, good precision, recall. 

Scores for Decision Tree:

Precision score - 75.9%
Recall score – 97%
Accuracy Score – 77.2%
