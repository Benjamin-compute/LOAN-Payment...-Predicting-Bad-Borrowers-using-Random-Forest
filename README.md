# Loan-Approval-Prediction-using-Random Forest

This project explores publicly available data for LendingClub.com (download [here](https://figshare.com/articles/dataset/Lending_Club/22121477/4?file=39316160)). 
Lending Club connects people who need money (borrowers) with individuals who have money (investors). The overarching idea is that investors want to invest in borrowers whose profiles have a high probability of repayment. 
Random Forest Classification Algorithm was used experimentally to create a model that will help predict this.
Model Performance: Overall accuracy was considered with priority given to F1-score and recall, since it is critical to identify bad borrowers.

## Data
The data size is 236,846 rows with 28 features, and after cleaning and feature selection, the model was trained using 236,840 rows with 16 features
This training data spans from January 2014 to June 2016 (2+ years)
The model was applied to a new dataset having 95,019 rows and spanning from July 2017 to December 2018 (1+ years)

## Features
    * total_acc:       The total number of credit lines currently in the borrower's credit file
    * pub_rec:         Number of derogatory public records
    * revol_bal:       Total credit revolving balance: 
    * revol_util:      Revolving line utilization rate, or the amount of credit the borrower is using relative to all available revolving credit.
    * int_rate:        Interest Rate on the loan, as a proportion (a rate of 11% would be stored as 0.11). Borrowers judged by LendingClub.com to be more risky are assigned higher interest rates.
    * dti:             The debt-to-income ratio of the borrower (amount of debt divided by annual income).
    * purpose:         A category provided by the borrower for the loan request (takes values like "credit_card", "debt_consolidation", "small_businesses", etc). 
    * mort_acc:        Number of mortgage accounts.
    * loan_amnt:       The listed amount of the loan applied for by the borrower. If, at some point, the credit department reduces the loan amount, it will be reflected in this value.
    * installment:     The monthly installments owed by the borrower if the loan is funded.
    * fico:            The FICO credit score of the borrower
    * pub_rec_bankruptcies:    Number of public record bankruptcies
    * open_acc:                The number of open credit lines in the borrower's credit file.
    * emp_length:              Employment length in years. Possible values are between 0 and 10, where 0 means less than one year and 10 means ten or more years.
    * time_to_earliest_cr_line:     The number of days the borrower has had a credit line.
    
    * loan_status (this is the response variable):     Indicator variable, telling whether the loan has been fully or not fully paid 

