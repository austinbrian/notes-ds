# Introduction to Inferential Statistics
----
### Descriptive Statistics
We've got data in front of us, and this describes the data
- Univariate statistics *(primarily concerned with distribution)*
   * mean
   * median
   * mode
   * skewness
- Bivariate statistics *(primarily concerned with relationship)*
   * correlation
   * covariance
- Multivariate statistics (3+)

### Inferential Statistics
Implies that a descriptive analysis isn't possible
-----

Samples -----> statistics; e.g., sample mean (x-bar)

Population ----> parameter; e.g., pop mean (mu - &mu;)

## Frequentist statistics
***Confidence interval:**** a range of values for a parameter
   * The Central Limit Theorem says that the set of all sample statistics (e.g., x-bar), that they will be *normally* distributed around the true population mean

***Hypothesis test:*** an inversion of confidence intervals, testing whether the null hypothesis can be demonstrated **false** under the conditions specified
1. Set up your hypotheses - null and alternative (the negation of null)
2. Gather data
3. Calculate test statistic:
   * t = (x-bar)-&mu;/(s(sample std dev)/sqrt(n))
4. Find your p-value
5. Conclusion based on predetermined alpha;
   * alpha is set as p<.05 or another value set by the industry
   * Examine the

Python script for t-testing
`stats.ttest_1samp(list,mean)`
