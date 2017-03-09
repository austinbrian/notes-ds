# Statistics and Numpy
------

## Statistics basics
* Descriptive statistics - describes a given sample
..* EDA = exploratory data analysis
* Inferential statistics - looks more broadly to make inferences about a population to generalize
..* confidence intervals
..* hypothesis tests

**statistic** - a function of the data
....takes in the values of the data, and outputs a number for us

**univariate** - one number of output given a set of numbers (e.g., mean, range, mode, etc.)
**bivariate / multivariate** - analysis on two sets of data (e.g., correlation)

## Measures of Descriptive Statistics
How many hours of sleep? 7
**Distribution**: the set of all possible values of a variable AND how frequently it takes on those values
..- used to summarize all the information you have without having to include all the information

*Measures of center* = mean, median, mode
mean - denoted by μ
median - denoted by M

*Measures of spread* = range, interquartile range, variance/standard deviation
..- IQR = 75th percentile - 25th percentile
..- variance / standard deviation
..... average distance from the middle
For a population: | For a sample
-----|------
`import numpy as np` | `import numpy as np`
`np.std(list)` | `np.std(list, ddof=1)`

A sample has degrees of freedom = n-1

## Skewness
*Right-skewed / Positively-skewed* = the tail on the right, median is less than the mean
*Left-skewed / Negatively-skewed* = tail on the left, median greater than the mean

------
# Numpy
