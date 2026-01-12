12/21/2025

# Ridge Regression
**Ridge regression*** addresses some of the problems of Ordinary Least Squares([[Least Squares]]) by imposing a penalty on the size of the coefficients. The ridge coefficients minimize a penalized residual sum of squares
	AKA L2 Regularization

Ridge Regression works very similar to Least Square method, but adds an $\alpha$ term into the equation in order to shift the slope and intercept
	Enables the line of best fit to be more generalizable, especially when looking at training vs testing datasets

So, instead of minimizing $\sum error^2$, it minimizes $\sum error^2 + \sum\lambda^2$, which includes the sum of squared coefficients

$$\underset {w} {min} ||Xw -y||\underset {2} {2} + \alpha|w||\underset {2} {2}$$
The complexity parameter $\alpha \ge 0$ controls the amount of shrinkage: the larger the value of $\alpha$, the greater the amount of shrinkage and thus the coefficients become more robust to collinearity

As the $\alpha$ term increases, the slope of the regression line decreases, becoming more horizontal and less sensitive to variations of the independent variable

```
from sklearn import linear_model
reg = linear_model.Ridge(alpha=.5)
reg.fit([[0, 0], [0, 0], [1, 1]], [0, .1, 1])
reg.coef_
reg.intercept_
```

https://www.youtube.com/watch?v=OEU22e20tWw

# Ridge Classification
The `Ridge` regressor has a classifier variant: `RidgeClassifier`
	AKA Least Squares Support Vector Machine(SVM)

This classifier first converts binary targets to {-1, 1} and then treats the problem as a regression task

For multiclass classification, the problem is treated as a multi-output regression, and the predicted class corresponds to the output with the highest value

Basically, the model makes 1+ lines as a line of best fit in order to separate data points on which group they fit into
	It draws lines in the sand as a means of organizing and separating data points that fall into different categories

`RidgeClassifer` can be significantly faster than `LogisticRegression` with a higher number of classes because it only needs to compute the projection matrix once

Same order of complexity as Ordinary Least Squares

Code: 
```
import numpy as np
from sklearn import linear_model
reg = linear_model.RidgeCV(alphas=np.logspace(-6, 6, 13))
reg.fit([[0, 0], [0, 0], [1, 1]], [0, .1, 1])
reg.alpha_
```
The `cv` attribute triggers the use of cross-validation with `GridSearchCV`