# System of Linear Vector Equations
A **linear system** is system of $m$ simultaneous equations in $n$ variables of the form
	Equations in a linear system of equations must have only coefficients and constants, meaning no exponents or logarithmic functions

The form for equations in a linear system are:
	$a_{11}x_1+a_{12}x_2 + ...+ a_{1n}x_n = b_1$
	$a_{21}x_2 + a_{22}x_2+..+a_{2n}x_n = b_2$

The process of condensing a matrix to the minimal amount of information required is converting the equations of a linear system into a **coefficient matrix**, then converting the coefficient matrix into an **augmented matrix**
	Linear System $\to$ Coefficient Matrix $\to$ Augmented Matrix

We can express a linear system in the form: $Ax = b$ where
$$A = \begin{pmatrix}
a_{11}&a_{12}&...&a_{1n}\\\\
a_{21}&a_{22}&...&a_{2n}\\\\
...&...&...&...& \\\\
a_{m1}&a_{m2}&...&a_{mn}
\end{pmatrix}$$
$$x= 
\begin{pmatrix}
x_1 \\\
x_2 \\\
... \\\
x_n
\end{pmatrix}$$
and 
$$
b =
\begin{pmatrix}
b_1 \\\
b_2 \\\
... \\\
b_n
\end{pmatrix}
$$
$A$ is the **coefficient matrix**
$x$ is the vector components
$b$ is the right side of the equations

$2x_1 + x_2 = 7$
$x_1 + x_2$  = 3

# Reduced Row Echelon Form 
A matrix is in **Reduced Row Echelon Form(RREF)** if:
	Each **pivot**(the leftmost non-zero entry in a non-zero row) is equal to 1
	Each pivot is the only nonzero entry in its column
	For each pivot, all pivots in the subsequent rows appear further to the right
	All rows of zeros are at the bottom

The first two conditions of RREF describe the Reduced aspect of the form, whereas the last two conditions describe the Row Echelon aspect of the form

**Pivot Columns** are columns containing a pivot

**Free Columns** are columns with no pivot

**Free Variables** are variables that can be assigned a arbitrary value, which allows for infinite solutions
	Basically, its when you put other components in the form at $x_a=kx_b$, making $x_b$ the free variable
	It means there are no pivots in its columns

A **rank** of a matrix $A$ is the number of pivot columns in the RREF of the matrix $A$

# Theorem 2.5: Solutions to Linear Systems
Consider a linear system of $m$ equations and $n$ variables with coefficient matrix $A$ and augmented matrix $A$. The system has
	No solutions, if the RREF of $A$ has a row $\begin{pmatrix}0&...&0&|&1\end{pmatrix}$(inconsistency)
	Exactly one solution, if the system is consistent and $rank(A) =n$
	Infinitely many solutions, if the system is consistent and $rank(A) < n$


# Resources
Khan Academy
https://www.khanacademy.org/math/linear-algebra/vectors-and-spaces/matrices-elimination/v/matrices-reduced-row-echelon-form-2

Basic & Free Variables
https://www.youtube.com/watch?v=j7hQ2dt2Z1g

Rank:
https://www.youtube.com/watch?v=cSj82GG6MX4
