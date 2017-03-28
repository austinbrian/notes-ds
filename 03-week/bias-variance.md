# Bias-Variance Tradeoff

**Bias**: Error that results from the correct value and the predicted value within our model; aka just residual error

**Variance**: Error due to the variability of a model prediction for a given data point

Calculating mathematically, combine three things:
- The sum of error between the predicted value and the actual value, squared -- **residual error**
- The range of predicted outcomes; so we want to look at the mean output of the model vs all the possible outputs -- **variance**
- an irreducible amount of noise


As model complexity increases:
- bias decreases
- variance increases

High bias, low variance = underfit
- model is a constant term, like y=4
Low bias, high variance = overfit
- highly complex model that hits all the points
