# Regression metrics
-----
## Key Ideas
1. R^2 is the most common
2. Sum of squares of error (SSE) = to to LOTS of metrics
  * also minimizes root means squared error
  * RSS = SSE = MSE = RMSE
3. Use-case/industry dependent


**Root means squared error**: the square root of the SSE / n

**R squared**: how much of the variance is explained by the model relative to the average of y (ybar)
  * R^2 = 1 - (sum of squared error/total sum of squares)

Root means squared error - returns a value in the units of the original dataset

## Loss Functions
* Loss functions are methods of evaluating a model that you want to minimize
* Ex:
  - Mean squared error
  - regularized function, which includes both MSE and a coefficient penalty

## Gradient Descent Algorithm
1. Pick a learning rate, &alpha;
2. Pick a starting point for a parameter, &beta;1,1
3. Check the value of a loss function at &beta;1,1
4. Figure out the direction that has the greatest downward slope
5. Re-calculate the loss function for a second &beta;1,2, which is &alpha; far away.
6. Stochastic gradient descent = at each step, choose a random size of &alpha;; helps avoid getting stuck in local min/max
