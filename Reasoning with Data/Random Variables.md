<u>Random Variable</u> is an outcome of a random phenomenon that takes numerical values

There are two types of random variables:
	<u>Discrete</u> is a random variable that can only take on 'separated' numerical outcomes
		Represented by a one-variable probability table or a relative-frequency histogram
	<u>Continuous</u> is a random variable which can take on an entire interval of numerical outcomes
		Represented by density curves that models a relative-frequency histogram

Binomial Conditions:
	the same fixed sample size,$n$, for every possible trial of the study
	Two Categories for each observation(Success/failure)
	The observations in the sample must succeed or fail independently of one-another
	Probability, $p$, of success must be same for each observation in the sample 

The last two conditions are guaranteed if random selection and population size is relatively large compared to sample size(10-20x)

Binomial Probability:
	P(exactly x success out of n) = (binomial coefficient)(overall success probability)$^\text{number succeed}$ (overall failure probability)$^{number fail}$ P() = $_nC_x*p^x*(1-p)^{n-x}$  

Binomial Coefficient
A whole number that represents the number of ways that $x$ identical items can be arranged among $n$ positions

$\frac{\text{repeated decreasing product of sample size down to 1}}{\text{[repeated decreasing product of number of successes, down to 1][repeated decreasing product of numbers of failures, down to 1]}}$ 
$_nC_x = \frac {n!}{x!(n-x)!}$

$0! = 1$ 
