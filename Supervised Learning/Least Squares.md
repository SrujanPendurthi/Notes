12/21/2025
# Concept

Intended for regression in which the target value is expected to be a linear combination of features.

**Features** are the measurable, individual characteristics, or attributes of the data used as inputs for algorithms to learn patterns and make predication
	Crucial for model performance and enable algorithms to understand relationships 
	*Examples: age, color, size, height, weight*

This means that the target value is expected to be related to features through a linear relationship

**Regression** is a statistical method for estimating the relationships between a dependent variable and 1+ independent variables
	Finds the line of best fit
	*Examples: predicting home price(dependent variable) using the size(independent variable)*
	
$$Y_i = f(X_i,\beta) + e_i$$
	$Y_i$ = dependent variable
	$f$ = function
	$X_i$ = independent variable
	$\beta$ = unknown parameters
	$e_i$ = error terms
$$\hat{y}(w,x) = w_0 + w_1x_1+...+w_px_p$$
$w$ = coefficient vector
$w_0$ = intercept

## Ordinary Least Squares

**Linear Regression** fits a linear model with coefficients $w = (w_1,...,w_p)$
to minimize the residual sum of squares between the observed targets in the dataset, and the targets predicted by the linear approximation
	Finds the minimum of the absolute value of the sum of differences of all the points and a given line fit in order to find the best line of fit
$$\underset {w} {min} ||Xw - y||\underset {2} {2}$$
Coefficient estimates for Ordinary Least Squares rely on the independence of features
	The *Independence of features* means that features must not have any relationships
	When features are correlated and some columns of the design Matrix $X$ have an approximately linear dependence, the design matrix becomes close to a singular and 
		As a result, the least-squares estimate becomes highly sensitive to random errors in the observed target, producing a large variance
This is called **Multicollinearity**, when 2+ predictor variables(features) are highly correlated

## Non-Negative Least Squares

It is possible to constrain all the coefficients to be non-negative, which may be useful when they represent some physical or naturally non-negative quantities

Linear Regression accepts a boolean positive parameter: when set to True

## Ordinary Least Squares Complexity
The least squares solution is computed using the singular value of $X$. If $X$ is a matrix of shape, the method has a cost of

Assuming that $n_{samples}\ge n_{features}$
$$O(n_{samples}, n_{features}),$$

# Code:
```
from sklearn import linear_model
reg = linear_model.LinearRegression()
reg.fit([[0, 0], [1, 1], [2, 2]], [0, 1, 2])
reg.coef_
reg.intercept_
```

Defines 'reg' as  a Linear Regression Model.
Then, defines the data points, coefficients, and intercept
# In Practice
Procedure for Least Squares Method:
	Count the data points and set them to $n$
	Find the $\sum x$ $\sum y$ , $\sum xy$, and $\sum x^2$
	Use the equations to find the slope and intercept
	$$Slope = \frac {n(\sum_{i=1}^{n} xy) - (\sum_{i=1}^{n} x)(\sum_{i=1}^{n} y)} {n((\sum_{i=1}^{n} x^2)-(\sum_{i=1}^{n} x^2))}$$
	$$Intercept = \frac {(\sum_{i=1}^{n} y)(\sum_{i=1}^{n} x^2) - (\sum_{i=1}^{n} y)(\sum_{i=1}^{n} xy)} {n((\sum_{i=1}^{n} x^2)-(\sum_{i=1}^{n} x^2))}$$
# Resources

Videos:
https://www.youtube.com/watch?v=P8hT5nDai6A