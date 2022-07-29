# Prosper Loan Data Exploration
## by (Ishola Olufunmi Abiodun)

## Description:
Banks lose a lot of money to several loans obtained by borrowers each year. Lots of banks have become insolvent due to various borrowers defaulting on their loans, some loans getting charged off and a lot more people repaying loans untimely. In this project, the loan dataset from Prosper would be explored and analyzed to determine the factors that influence the end status of loans and predict the possibility of a borrower repaying their loan.

## Dataset

> The [loan dataset from prosper](https://www.google.com/url?q=https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv&sa=D&ust=1581581520570000) consists of 113937 loans(rows) and 81 variables regarding each loan, including: LoanOriginalAmount, Term, BorrowerRate, etc. The feature documentation detailing each variable meaning can be found [here](https://www.google.com/urlq=https://docs.google.com/spreadsheet/ccckey%3D0AllIqIyvWZdadDd5NTlqZ1pBMHlsUjdrOTZHaVBuSlE%26usp%3Dsharing&sa=D&ust=1554486256024000).
34 rows were dropped from the dataset including null values and outliers. Likewise columns with incomplete data (some columns only contain data for certain years) and those not needed for analyses were dropped.
Also, for easy analyses, map function was used to map the names of certain values in some variables to names more understandable and at the same time did not change the authenticity of the data.

## Summary of Findings
> After successfully wrangling the data, I started by exploring the variables individually, then took it down to paired exploration.

> During the exploration of the dataset, I observed that some variables wholly influenced loan status while some unless explored with other variables, they did not affect outcome of loans. The loan amount seemed slightly correlated with loan status when compared without any other variables. But with other variables and loan amounts, there seemed to be a much more stronger correlation. The number of investors as a standalone variable seemed strongly correlated with loan status compared to when explored with other variables. There also seemed to be a high correlation between amount invested by friends and loan status as loans with much invested amount tend to be more completed than those with low invested amount. The term and quarter variables as standalone variables and even when paid with other variables did not seem correlated with loan status.

Exploring the non-interest variables, the annual percentage rate and the interest rate had a very strong correlation and it seemed the interest rate was the biggest driver of annual percentage rate admist other loan charges. The monthly loan payment also seemed very correlated with the loan amount, and as loan amount increased, monthly loan payment too increased.
From the exploration, it was observed that delinquencies- current delinquencies and delinquencies last seven years had strong correlations with loan status, and borrowers with high delinquencies had minimal chances of completing their loan payments. This is a little similar to the debt-to-income variable against loan status, as a somewhat strong correlation also existed between them and a high debt-to-income ratio with paired with other negatives features might signify lower ability to repay loans.
The influence of the Income range variable on loan status was more obvious when paired with loan amount and a strong correlation seemed to exist between them too.
It was also observed that borrowers who paid about ten percent of the amount borrowed every month had higher chances of completing their loans.

## Key Insights for Presentation

For the presentation, I focused on the variables that influenced loan status either singly or when paired with other variables.
I started by introducing my main variable of interest- loan status, its distribution across the dataset and took it down to single factors that influenced it down to mutiple factors.

I started with a bar plot exploring the distribution of the loan status as a categorical variable, then I presented a histogramic distribution of loan amount; the numerical variable of interest. I then moved to the exploration of the distribution of loan amount against loan status, then distribution of another variable strongly correlated with loan amount- BorrowerAPR. I tweaked my visualization a little by resetting the orders of the plots and figure sizes of loan amount against loan status and APR against loan status.

I then used two plots from part 1 exploration to depict the relationship between loan status, loan amount, investment amount and income range variables.

## Conclusion:
Some variables singly or in pairs influence if a borrower would be able to repay a loan or not.


Having knowledge about the repayment capacity of a borrower would help lenders (banks) know what to expect and if they should give out the loan, reduced the amount or not give out at all.
