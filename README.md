Problem Statement: 50 companies with there operational spend and what was the profit for that company, analyse the companies and tell the VCs to which companies to invest on the basis of profit. Build a model for such case
Multiple Regression: Combination of multiple Linear Regression
Assumptions for Linear Regression

Linearlity
Homoscadisticity
Multivariate Normality
Independence of Error
Lack of Multicolinearity
Building a Model
All In
Backward Selection
Forward Selection
Bidirectional Selection
Score Comparison
All In
Use all the variables to build the model, this method is not suggested. This is either asked by the client to use these variables or someone with better domain Knowledge
Backward Selection
Step 1: Select a significant level to stay in the model
Step 2: Fit the model with all predictors
Step 3: Consider the predictor with higest p-value and if p-Value is greater than Significance Level then move to step 4. Otherwise go to finish model by using all the variables with right significance level
Step 4: Remove the predictor
Fit the model with that predictor
Forward Selection
Select a significance level to enter the model
Fit all simple linear regression models y~Xn and select one with the lowest P-value
Keep this variable and fits all possible models with one extra predictor added to the one(s)
Consider the predictor with lowest p-value. If P < Significance Level then go to step 3 other wise finish the model
Bidirectional Elimination
Step 1: Select significance level for the variable to stay (SL=0.05) and to enter (SL= 0.05)
Step 2: Perform the next step of Forward Selection (New variable must have p<SL-enter)
Step 3: Perform all steps of backward elimination (Old Variables must have P<SL-stay)
Step 4: No new variables can enter and no old variabels can exit, finish the model
All Possible Model
Step 1: Select Criterion of Goodness of model

R square – Higher the Better
It tells about the goodness of the fit. It ranges between 0 and 1. The closer the value to 1, the better it is. It explains the extent of variation of the dependent variables in the model. However, it is biased in a way that it never decreases(even on adding variables).

Adj Rsquare – Higher the Better
This parameter has a penalising factor(the no. of regressors) and it always decreases or stays identical to the previous value as the number of independent variables increases. If its value keeps increasing on removing the unnecessary parameters go ahead with the model or stop and revert.

F statistic – Higher the Better
It is used to compare two variances and is always greater than 0. It is formulated as v12/v22. In regression, it is the ratio of the explained to the unexplained variance of the model.

AIC and BIC – Lower the Better
AIC stands for Akaike’s information criterion and BIC stands for Bayesian information criterion Both these parameters depend on the likelihood function L.

Skew – Lower the Better
Informs about the data symmetry about the mean.

Kurtosis – Higher the Better
It measures the shape of the distribution i.e.the amount of data close to the mean than far away from the mean.

Omnibus –
D’Angostino’s test. It provides a combined statistical test for the presence of skewness and kurtosis.

Log-likelihood –
It is the log of the likelihood function.

Step 2: Construct all possible regression models: (2^N)-1 total combination

Step 3: Select one with the best Criterion
