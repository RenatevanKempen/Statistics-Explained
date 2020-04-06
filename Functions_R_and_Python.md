# Equivalence between distribution functions in R and Python


Thanks to [Alberto Torres Barrán](http://albertotb.com/Equivalence-between-distribution-functions-in-R-and-Python/)


The name for the different functions that work with probability distributions in R and SciPy is different, which is often confusing. The following table lists the equivalence between the main functions:

 |  R	  | SciPy	  | Name  |
 |-----|------|-----|
 | dnorm()  | pdf()	  | Probability density function (PDF)         |
 | pnorm()	| cdf()	  | Cumulative density function (CDF)          |
 | qnorm()	| ppf()	  | Percentile point function (CDF inverse)|
 | pnorm(lower.tail = FALSE)|	sf()|  Complementary CDF (CCDF) or survival function|
 | qnorm(lower.tail = FALSE)|isf()|  CCDF inverse or inverse survival function |
 |rnorm() | rvs()	| Random samples |


Note: in R the names are ilustrated using the normal distribution. 
Functions for other distributions can be constructed keeping the first letter of the name and changing the name of the distribution, 
for example, for the gamma distribution: dgamma(), pgamma(), qgamma() and rgamma().
