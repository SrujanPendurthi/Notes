**Population** is the complete set of people or objects of interest, or the infinite set of all possible values if the same person or item were repeatedly measured in the same way
	Measurements vary(from individual to individual, or from moment to moment)
	Usually, a population cannot be measured entirely(this necessitates sampling and inference), because it is usually too costly or time consuming to measure every such individual or item(or because it is impossible to make an infinity of measurements on the same object)

**Sample** the subset(sub-collection) of the population for which data can actually be obtained in a study
	Samples vary one to the other(and hence a sample statistic varies from sample to sample)
	Samples obtained using probability methods allow the use of probabilistic inference techniques

**Parameter** is a fixed(but usually unknown) number summarizing some feature of a population
	Two very elementary examples of parameters are average or proportion
	A parameter is usually unknown(this necessitates estimation and inference), since an entire population can usually never be measure

**Statistic** is a computed number that summarizes sample data in some appropriate way, which estimates a parameter
	For any given study, the statistic is the best *estimator* of the corresponding parameter
	the statistic varies from sample to sample(and hence it is an *imperfect* estimator of the parameter)
	if the source of the variation of the statistic is *random*, then the statistic has a *probability distribution*

**Inference** is specifying the estimate of an unknown parameter
	If the statistic was a random variable and if the probability distribution of the statistic can be determined, then the inference is *probabilistic inference* and can include probability measures or margins of error

# Identifying Data Types
**Individuals** is the people or objects described in the dataset

**Variables** is a characteristic which varies from person to person, typically be identified by a column in a 
	*Examples: sex, age, ethnicity*

**Quantitative** is a naturally numerical; represents different magnitudes
**Categorical** is not naturally numerical
	AKA: Qualitative

Shape: Modality and skews
Center: What is the typical value?
Spread: Within about how many units do the majority of values tend to lie from the average?
Outliers: Any values that seem to be suspiciously un-like the majority,

# Representations of Data
Frequency Tables are an example o distribution
Relative Frequencies/Percent Frequencies
Frequency Bar Graph for Categorical Data
Frequency Pie graph for Categorical data

# Standard Deviation
The greater the spread, the greater the value of standard deviation
Defined to be a positive number with the same units of data
Roughly $\frac{2}{3}$ of the values will be within one standard deviation

The equation below is the sample standard deviation, where you find the absolute difference between a data point and the mean
	$$S = \sqrt\frac{\sum_{i=1}^n(X_i-\bar{X})^2}{n-1}$$	The equation below is the sample population deviation, where you find the absolute difference between a data point and the mean
	$$\sigma = \sqrt\frac{\sum_{i=1}^n(X_i-\mu)^2}{N}$$
The standard deviation is a statistic whereas the population standard deviation is a parameter

**Variance** is the square of standard deviation

# The Boxplot
**Median** is the $50^{th}$  percentile
$Q_1$ is the 25% percentile, first quartile
$Q_3$ is the 75% percentile, third quartile
**Inter Quartile Range(IQR)** is $Q_3 -Q_1$, telling us how many units the middle half of the data range over and is a rough measure of data spread although not accurate

The Boxplot is a type of graphical display of the five-number summary of quantitative data
