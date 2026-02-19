**Relationship** exists between two variables if knowledge of the first variable tells you something about the value of the second variable that you would not know without that knowledge; in particular, a relationship is when particular values of the second variable are more likely to occur with certain values of the first variable
	AKA Association

# Contingency Tables
Cross-tabulation or two-way tables
Scatter-plots for displaying and exploring quantitative relationships
	direction, form(Linear vs 'other', strength), deviation(outliers)

# Pearson Correlation Coefficient
A unitless number that measures the *direction* and *strength of the linearity* between two quantitative variables

Characteristics of the Pearson Correlation Coefficient:
	Unitless, between -1 and 1
	the sign matches the direction of the relationship;
	Magnitude measures the degree of linearity of relationship
			Closer to zero, meaning not strong relationship
			Farther from zero, meaning strong relationship
	Only appropriate and  meaningful if the relationship is linear
	Not resistant to outliers or skews


Sample Pearson Correlation Coefficient(statistic)
$$R = \frac{\frac{1}{n-1}\sum_{i=1}^n(X_i-\bar{X})(Y_i - \bar{Y})}{S_xS_y}$$
Population Pearson Correlation Coefficient(parameter)
$$\rho= \frac{\frac{1}{N}\sum_{i=1}^n(X_i-\mu_X)(Y_i - \mu_Y)}{\sigma_x\sigma_y}$$
The quantity in the numerator is called **covariance**

**Residual(Error)**
	the vertical distance from point to line
	the observed $y$ minus the predicted $y$
	$y - \bar{y}$
	measure of how good or bad the line predicts the $y$ values. if the line is a good model of the data, the residuals should be small.

**The Meaning of $R^2$**
R is a measure of the linear direction and linear strength of quantitative association of the sample

R also appears as part of the formula for the slope regression line:
	Also, it arises a third way: Its square is a percentage measure of explanatory power

**$R^2$** as a percentage is the percent of variation in $Y$ predicted by the linear relationship with $X$


# Cautions with Correlation and Regression
Correlation and regression are only for linear relationships
Cannot extrapolate with high levels of confidence, but meaningful within the scope of $X$
	*Extrapolation* is using a model to make a prediction far outside of the scope of the $X$ values in the data that produced the model
Correlation is not the same as Causation

# Resources
[[Least Squares]] Least Ordinary Squares Notes