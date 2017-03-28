# Regularization
------

**Overfitting**
* Occurs because there are too many variables specific to the dataset
* Often happens with very *wide* datasets, with a lot of features, but not a lot of observations

**Bias**
- Describes the tendency to miss existing data points in a model

**Variance**
- The changes in predicted values for each x, basically the wildness of the line

## Linear regression
- Low variance, but high bias
- Doesn't tend to overfit
- Causes of overfitting include:
  - use of irrelevant features, especially when the number of features approaches the number of observations
  - correlated features
  - large coefficients

Regularization is a method of constraining the size of coefficients such that features that have less explanatory power ultimately go to zero.

## But how?
Using a loss function that takes into account both the residual sum of squares as well as the size of the coefficients themselves

Coefficients are tuned by &lambda; which penalizes the total size of all the coefficients
- Also, holy shit, if two features are dependent, it will reduce the SSE and the value of the coefficient concurrently if one of the dependent variables are reduced to zero

**Ridge regression** == l2_norm
- &lambda; tunes the sum of each of the coefficients squared
- the shape of the "penalty budget" is circular

**Lasso regression** == l1_norm
- &lambda; tunes the sum of each of the absolute values of each coefficient
- less forgiving of nonzero coefficients; it drives coefficients toward zero
- shape of penalty budget is linear, being absolute value

&lambda; is also described by &alpha; which is just 1/&lambda;
