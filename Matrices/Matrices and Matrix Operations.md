# Matrix
**Matrix** is an $m * n$  rectangular array of real numbers with $m$ rows and $n$ columns

The entries of a matrix are the individual numbers in the matrix

The set of all $m * n$ matrices is denoted $\mathbb{R}^{m*n}$

$$A =  \begin{pmatrix}
a_{11} & a_{12} & a_{13} \\
a_{21} & a_{21} & a_{21} \\
a_{n1} & a_{n2} & a_{n3} \\
\end{pmatrix}$$

Vectors are just special kinds of matrices
	A **column vector** with $m$ components is a $m * 1$ matrix 
	A **row vector** with $n$ components is a $n * 1$ matrix 
	A real number is a little $1*1$ matrix  

# Matrix Operations
Let $A,B \in \mathbb{R}^{m*n}$ and $k \in \mathbb{R}$
*Matrix addition*: $A + B$ is the matrix
	Must have the same dimensions
	Adding corresponding entries of $A$ and $B$
*Scalar Multiplication*: $k * A$ is the matrix
	scalar $k$ is distributed across to all entries of the matrix $A$
*Multiplying a matrix by a vector*:
	Let $A \in \mathbb{R}^{m*n}$ and $\vec{v} \in \mathbb{R}^{n*1}$, where $A = \begin{pmatrix}\vec{r}_1\\\vec{r}_2\\\vec{r}_3\end{pmatrix}$. Then, 
	$$A\vec{v} = \begin{pmatrix} \vec{r}_1 \cdot \vec{v} \\ \vec{r}_2 \cdot \vec{v} \\ \vec{r}_3 \cdot \vec{v} \\
		\end{pmatrix}$$
	$\vec{r}_1$ is a row vector which is doing the dot product with the vector $\vec{v}$, returning a column vector, so the form is $v_1\vec{c}_1 + v_2\vec{c}_2 + ... + v_n\vec{c}_n$ 
	This is how linear systems of vectors work because it is in the form, $A\vec{x} = \vec{b}$  
	You can either do this operation by row or columns
*Matrix multiplication*:
	Let $A$ be a $m*n$ matrix and $B$ be a $n*p$ matrix.
$$A =
\begin{pmatrix}
\vec{a}_1 \\
\vec{a}_2 \\
\vec{a}_m \\
\end{pmatrix}$$
$$B = 
\begin{pmatrix}
\vec{b}_1 & \vec{b}_ 1& \vec{b}_p
\end{pmatrix}$$

 The product of $AB$ is the $m*p$ matrix:
$$AB = 
\begin{pmatrix}
A\vec{b}_1 & A\vec{b}_2 & A\vec{b}_p
\end{pmatrix}$$
$$AB =
\begin{pmatrix}
\vec{a}_1\vec{b}_1 & \vec{a}_1\vec{b}_2 & \vec{a}_1\vec{b}_p \\
\vec{a}_2\vec{b}_1 & \vec{a}_2\vec{b}_2 & \vec{a}_2\vec{b}_p \\
\vec{a}_m\vec{b}_1 & \vec{a}_m\vec{b}_2 & \vec{a}_m\vec{b}_p \\
\end{pmatrix}$$
	Note this is only defined if number of columns of $A$ are the same as the number of rows of $B$. $A = m*n$ and $B = n*p$, so $AB = m*p$


*Matrix Powers*:
	Let $A \in \mathbb{R}^{m*n}$ be a square matrix, with an equal number of rows and columns, and $k$ be a positive integer. Then $A^k$ is the product of A with itself $k$ times