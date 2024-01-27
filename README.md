# Introduction
Bankrate was founded in 1976 as Bank Rate Monitor, a print publisher for the banking industry. When you visit Bankrate.com, the reviews, guides and educational content have been developed by leading personal finance experts. Bankrate’s product comparison tools, calculators and educational content help over 100 million consumers make smarter financial decisions each year. One area Bankrate specializes in is personal loans. Bankrate’s goal is to help match the best lending partner for each individual customer. To do that, we collect information about the customer to understand who would be the best fit. We want to maximize the likelihood someone will be approved for the loan at the best “deal” possible. In this case, let’s imagine we have three lending partners, “A”, “B”, and “C”. In this scenario, let’s imagine that each lender is providing the same offer. However, for each approval, lender A provides us $250, lender B pays us $350, and lender C pays us $150. The business team has recently collected this data and has asked you to help make sense of it. They want to know if they can increase revenue per application by matching certain groups of customers to specific lenders. 


# Which variables are the most helpful in understanding if a customer is going to be approved or denied for a loan?
Utilizing random forest, the top five most important variables for customer loan acceptance, from most important to least important, are "Fico_score", "Fico_Score_group_fair", "Monthly_Gross_Income", "Monthly_Housing_Payment", "Fico_Score_group_poor". It is important to note that random forest results do not tell us in what direction (positive, negative) the independent variables are impacting customer loan application acceptance.  


# What is each Lender’s average approval rate and how does their revenue per approval differ? Are there any clear differences between the three different lenders on what type of customers they approve?
The average approval rate for each lender is as follows; Lender A = 10.97%, Lender B = 7.13%, Lender C = 17.06%. The revenue per approval by lender is as follows; Lender A = $250, Lender B = $350, Lender C = $150. Lender A mainly approves customers who are of full time working status and gives out a broader range of loan amounts. Lender B approves people with higher FICO scores (average of 732.11) and a smaller standard deviation than lenders A and B which means Lender B is far more selective in terms of FICO score. Lender B also accepts people with a higher monthly income (average of $8,053). Lender C is much more lenient when it comes to approving loans compared to their counterparts. Lender C approves an average FICO score of 674.77, an average monthly gross income of $6,322.16. However, Lender C seems to care far more than Lender B if the loan applicant is of Full time working status.


# Are there groups of customers that would be a better fit for a different lender? How much incremental revenue could we have made if we matched certain groups of customers more appropriately?
Using the median of FICO_score, Loan_amount, and Montly_gross_income for each lender, I calculated total revenue generated. I then compared unmatched customers to the median of the previously stated variables and if they exceeded all of criteria, then I deemed the customer as a missed opportunity. Overall, I found that due to missed potential matches, the revenue missed out by lenders are as follow; Lender A: $759500.00, Lender B: $985950.00, Lender C: $1686900.00. 


# Conclusion
Bankrate, originating as Bank Rate Monitor in 1976, has evolved into a leading financial platform with content curated by experts. Focusing on personal loans, the objective is to enhance revenue per application by strategically aligning customers with the most compatible lender. Leveraging random forest analysis, critical variables influencing loan approval, such as "Fico_score" and "Monthly_Gross_Income," have been identified. While the analysis provides insights into lender preferences, the revenue potential is further illuminated by revealing missed opportunities, with projected gains of $759,500 for Lender A, $985,950 for Lender B, and $1,686,900 for Lender C, underscoring the impact of precise customer-lender matching on financial outcomes.
