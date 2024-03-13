# MODEL FOR REDUCING RISK WHEN GRANTING FINANCIAL LOANS

# Problem

Given a huge sum of money to be given for loans, it can become a little tricky to decide on what loan application to select based on the information shared by the applicant (in the application). Lenders usually look at a measuring unit called a recovery factor which determines whether a borrower would be able to return the loaned amount in the given period with a given interest rate. Due to COVID, various businesses have faced and, in fact, still face financial problems resulting in a not-so-appealing recovery factor. The current situation has made it a little stressful for lenders to approve loans. A wrong approval can hinder efficiency in workflow and affect the methods of assessing loans in the future.
This is where the proposed solution comes into play. The main aim is to offer an application to financial companies that uses machine learning methods to transform and handle large
and complex datasets and turn them into valid strategies that allow greater access to loans for people that are qualified while lowering the financial risk of lenders. The application would
help lenders make an informed decision by only suggesting cases fitting the respective risk appetites and commercial objectives.

# Objective

The main aim is to offer an application to financial companies that uses machine learning methods to transform and handle large and complex datasets and turn them into valid strategies that allow greater access to loans for people that are qualified while lowering the financial risk of lenders. The application would help lenders make an informed decision by only suggesting cases fitting the respective risk appetites and commercial objectives.

To accomplish this a dataset from FICO was obtained containing loan application information and classification of whether the application was good or bad.

# Data Collection

The Home Equity Line of Credit (HELOC) dataset was sourced from FICO community. It can be found on the Explainable Machine Learning Challenge. The dataset contains a line of credit normally provided by a bank as a percentage of home equity. Applicants solicited personal credit from $5,000 to 150,000. In addition, the dependent variable to predict is a binary variable called ‘Risk Performance’ whose value “Bad” means that a person was 90 days past due or more. The value “Good” indicates that an individual made on time its payments/deposits.

# Solution 

The data set contains binary target variables concerning their risk performances i.e., either “good” or “bad.” Thus, the initial problem is to build a model to classify these applications. Hence, a logistic regression algorithm was chosen. Interestingly, this algorithm is a classification problem. This algorithm comes from the fact that it not only classifies the target variable such as 1’s and 0’s and also gives the probability of the observation set to be 1’s or 0’s. 
Finally, model build training was trained on 70% of the dataset using Logistic Regression and was tested on the rest 30% giving the average accuracy score of 72.43% after 5-cross validations. 

# Dashboard
Google studio host the application, where at the top middle, the user can select any applicant ID and automatically it will visualize its risk probability for the lender. On the other hand, the table shows the 10 groups of applicants (deciles) with lower and maximum risk probability of making their payments/deposits on time. Another example is the bar chart. It shows the maximum risk that a lender could have on each group of people.  See the image  called lender’s risk model below. 

![image](https://github.com/eloisjr/Dashboard_Lenders_risk_probability/assets/81710422/5edf4045-36ba-4cf7-b997-647ff4e62589)




Lender’s risk model can be found in the link below.

https://lookerstudio.google.com/u/0/reporting/d7085977-5870-49ff-82e5-0ab447bc8839/page/Gke4C

