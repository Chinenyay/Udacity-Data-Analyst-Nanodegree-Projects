# (Prosper Loans Dataset Exploration)
## by (Jennifer Chinenye Umoke)


## Dataset


I analysed the Prospa Loans Dataset which contains information about 113,937 loans listed on the American crowd-lending site from 2005 to 2014. It contains 81 datapoints on the loans, borrowers and investors. The features I selected for investigation are as follows:
- loan status
- borrower APR
- borrower rate
- listing category
- occupation
- isborrowerhomeowner
- income verifiable
- stated monthly income
- loan original amount
- total trades
The dataset is available here: https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv


## Summary of Findings

> Summarize all of your findings from your exploration here, whether you plan on bringing them into your explanatory presentation or not.
Commencing with univariate exploration, I found that there were high outliers in the monthly income values. The maximum value was 1.7 million dollars per month which I removed from the dataset in the exploratory phase because it shifted all the values extremely to the right. Following this, I limited the income values to between $500 - $50k and applied a log transformation which revealed a normal distribution with a slight right skew. This is because most of the income values were clustered around $500 to $50k dollars.
The number of home owners in the dataset was slightly higher than non-home owners and most of the borrowers had submitted documentation to verify their monthly earnings. 

I also found that the most common use for loans was debt consolidation, which also correlated with an average of 20 tradelines per borrower and the highest loan amount was $35k. Tradelines, recorded in the dataset as totaltrades, represents the number of credit lines or accounts that a borrower has on their credit profile. These two findings revealed a high level of indebtedness among borrowers. Furthermore, I found that borrowers with a higher debt to income ratio struggled to pay their loans and had the highest rate of deliquency, and invariably there was a positive relationship between high income and repayment. Also, the best borrowers were judges. Only one borrower who worked as judge had defaulted by 1 - 15 days. Additionally, lower value loans had a higher charge-off rate than higher value ones. 

I also found that APR and Interest Rate were highly correlated. This was however to be expected since interest rates are calculated as part of APR and should move in the same direction. However, the lowest interest rates were given for loans that did not have any stated uses.


## Key Insights for Presentation


For my key insights I focused on the relationship between occupation, income and loan status. Generally, borrowers with a higher debt-to-income ratio were more likely to default on their loans. Students were the most deliquent low income borrowers while entrepreneurs were the most common high income borrowers. 
I also found it interesting that the lowest APRs were being given for loans whose uses were not provided, which I think might have a negative effect on profitability of the loans for investors. Finally, debt consolidation being the most common loan use showed a high level of indebtedness among borrowers. 