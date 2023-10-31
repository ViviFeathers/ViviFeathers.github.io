# Some Thoughts about Regression Model Variable Selection
Based on my own experiences, varaible selection for fitting a regression model can't be perfect most of time. 
There are some steps I follow when select variables.

## Step one, background information
In my daily work, we fit model using data from an observational study cohort to investigate the asscociations between couple of vairables and the outcome that we are interested in. We usually do some literature reviews to get some background knowledge about the outcome, and know it usually relates to several variables. Besides, we are interested to see if there are other variables related to the outcome, so we bring up hypothesis for those addtional variables and include them together with the literature review ones into the variable pool.

## Step two, EDA
After decide our variable pool, we check the normality, center and spread of each numeric variables, also plot their correlation between each other. That way, we will know if we need to center certain variables or remove some variables because of collinearity.

## Step three, backward selection
The initial model will have all the variables we processed and kept, then we use backward elimination method to reduce the variable number since this method deletes variable one by one from the full model until all remaining variables have some significant contribution to the outcome, it reduces the multicollinearity problem also resolvse the possible overfitting issue.

## Step Four, check adjusted R-squared, AIC, BIC and plot residuals
Get an idea about the values of adjusted R-squared, AIC and BIC, then plot the residuals to see if the residuals follow a no-parttern distribution. If they do, the model fitting is mostly done unless we want to include more variable and investigate.
If the residuals have certain parttern, we will include all polynomial terms as well as interaction terms into our model and do backward elimination again.
Remember to check the values of adjusted R-squared, AIC and BIC, if they are much better than the old model, we will keep the high level terms, if they are slightly better, we might remove high level terms to avoid overfitting, also high level terms are not as easy to interpret as low level terms.

