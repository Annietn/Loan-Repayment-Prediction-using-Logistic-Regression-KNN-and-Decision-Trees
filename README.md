# Loan-Repayment-Prediction-using-Logistic-Regression-KNN-and-Decision-Trees

In lending industry, a lender gives a loan to a borrower, who is then expected to repay his/her debt. However, there is always a risk that the borrower is unable to repay the loan, causing the lender’s financial losses. Thus, determining the likelihood of loss on a loan is necessary for lenders in making a lending decision. In this dataset, I carried out a credit risk assessment by using logistic regression, KNN trees, and decision trees model. Using not.fully.paid as the dependent variable, I predict a borrower’s ability to pay off their loan based on his/her financial information, namely, his/her purpose of the loan, his/her FICO score, the number of his/her has had a credit line, his/her amount of used and unpaid credit card at the end of billing cycles, etc. as well as the lender’s interest rate and installment. The dataset contains 9578 rows and 14 variables, and there is no sign of any outliers. Although the three models show their advantages in predicting the possibility of borrower fully paying off the loan, logistic regression has the highest accuracy rate. In addition, logistic regression is the only model that shows the interrelationship between the borrower’s financial historical information and their ability of paying off the loan.  Specifically, the logistic regression model shows that the borrower's number of inquiries by creditors in the last 6 months, the number of days he/she has had a credit line, his/her purpose to take loan to set up a business, along with his/her other purposes of taking loan, are the most significant factors that would increase the risk of his/her inability of paying off a loan. On the other hand, his/her self-reported annual income would decrease the risk of that he/she would not pay off a loan. To improve the logistic regression model, in the future, I would remove all the insignificant variables and then run the model with all the significant variables.

credit.policy: 1 if the customer meets the credit underwriting criteria of LendingClub.com, and 0 otherwise.
purpose: The purpose of the loan (takes values “credit_card”, “debt_consolidation”, “educational”, “major_purchase”, “small_business”, and “all_other”).
int.rate: The interest rate of the loan, as a proportion (a rate of 11% would be stored as 0.11). Borrowers judged by LendingClub.com to be more risky are assigned higher interest rates.
installment: The monthly installments ($) owed by the borrower if the loan is funded.
log.annual.inc: The natural log of the self-reported annual income of the borrower.
dti: The debt-to-income ratio of the borrower (amount of debt divided by annual income).
fico: The FICO credit score of the borrower.
days.with.cr.line: The number of days the borrower has had a credit line.
revol.bal: The borrower’s revolving balance (amount unpaid at the end of the credit card billing cycle).
revol.util: The borrower’s revolving line utilization rate (the amount of the credit line used relative to total credit available).
inq.last.6mths: The borrower’s number of inquiries by creditors in the last 6 months.
delinq.2yrs: The number of times the borrower had been 30+ days past due on a payment in the past 2 years.
pub.rec: The borrower’s number of derogatory public records (bankruptcy filings, tax liens, or judgments).
