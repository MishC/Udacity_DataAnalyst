
Dataset
# Loan Data Exploration

The dataset from the Prosper attributes of 113,937 available dated in 9.11.2005 - 10.3.2014. Dataset contains 81 variables on each loan, but only some have been used for analysis. 

## Summary of Findings

I have find that number of borrowers via Prosper have increased from 2005 to 2014. In 2005 were interested more than 5000 borrowers while in 2013, there is more than 35000 borrowers via Prosper. This growing tendency is characterized for the whole period, except the years 2009 and 2010.

In my analysis I was searching the ansers for these questions:

### What factors affect a loan’s outcome status?

I studied how is loan status affected by the current amount delinquent, loan original amount, stated monthly income.
I have found that those, who have the highest amount delinquent are "Defaulted". Highest loan original amount belongs to loan status "Current" followed by "Charged-off".
Borrowers with the highest income belong to the status "Current" and with the lowest income to "Defaulted". 
Furthermo,re I have found that from those, who are "charged-off", have 30.3% a public record in the last 10 years. 

### What affects the borrower’s APR or interest rate?

The Borrower's APR reflects borrower's prosper rating. These 2 variables are strongly negatively correlated. The Borrower's APR reflects borrower's prosper rating.
As expected, With higher APR, lender yield is increasing appropriately.

Furthermore, Borrower's APR is influenced by the loan original amount and available bank credit in the time when loan was created.

### Are there differences between loans depending on how large the original loan amount was?

The highest mean loan original amounts have the borrowers with the loan status Current and with the highest ratings (AA, A, B)
I have studied completed loans, those which are terminated. Longest period loans have those who are "Defaulted" and the shortest period loans have borrowers with the loan status "Completed" and with the highest ratings (AA, A, B).
The most of borrowers have salaries in range $0-50000 and most common loan original amount is less than $5000.

## Key Insights for Presentation

There are 2 presentations called  exploratoration.html and explanation.html
I generated them by this command:

jupyter nbconvert explanation.ipynb --to slides --post serve --template output-toggle

jupyter nbconvert exploration.ipynb --to slides --reveal-prefix reveal.js --post serve
