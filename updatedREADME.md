# King County Housing Regression Model
### Author: Ryan Sims

Given housing data from King County, Washington, generate a linear regression model that can predict house prices as accurately as possible.

The data used for this project was the King County, Washington housing data.

## Methods:

### 1) EDA
> Begin with looking at the how each of the raw columns correlate with eachother.  This will help determine if there is a linear relationship and if any of the columns have potential multicollinearity issues.
> Once the relationships of the raw data is inspected, perform any cleaning, scaling, and feature engineering.

### 2) OLS and LinearRegression
> The OLS model from statsmodels was used to provide different metrics on model, mainly evaluating the statistical significance and the R^2.  
> Scikit-learn LinearRegression was used to determine the mean squared error metric to determine how well the model generalized from training to test data.

## Results
> The model returned a weak R^2 value of 0.66.  This states that 66% of the change in price could be explained by the change in the features.  The MSE did show that the model generalized well, which means it would be able to reproduce similar results from new data.

## Recommendations
> I would recommend to pay attention to the distributions of the raw data.  The skewness and outliers will affect the regression model.  I used scaling and normalizing in my feature engineering which could prove to have weakened the model.  Depending on the skewness of some of the features, log transformations might have aided in a more accureate regression model.

