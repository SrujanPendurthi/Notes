<u>Theorem 10.1: Test for Linear Independence in $\mathbb{R}^n$</u>

Let $v_1,...,v_k \in \mathbb{R}^n$ be vectors and $A$ be the matrix $v_1,...,v_k$ as its columns
	If the rank of $A$ is equal to $k$, then the vectors $v_1,...,v_k$ are linearly independent
	If the rank of $A$ is less than $k$, then the vectors $v_1,..,v_k$ are linearly dependent. In this case, the vectors corresponding to the pivot columns of the RREF of $A$ make a linearly independent set which has the maximum size of any linearly independent set of vectors from $v_1,...,v_k$

<u>Lemma 10.2: Linear Dependence Lemma</u>
Suppose $v_1,...,v_n \in V$ are linearly dependent. Then there exists a vector $v_k$ in the list such that:
	$v_k \in span(v_1,...,v_{k-1},v_{k+1},...,v_n)$
	$span(v_1,...,v_{k-1},v_{k+1},...,v_n) = span(v_1,...,v_n)$

# Bases
A <b>basis</b> of a vector space $V$ is a linearly independent list of vectors in $V$ that spans $V$
	Examples: $\hat{i},\hat{j}$ 

The <b>standard basis</b> of $\mathbb{R}^n$ is the basis $e_1,...,e_n$ of vectors in $\mathbb{R}^n$ defined as follows:
$$e_1 = \begin{pmatrix}1\\0\\0\\...\\0\end{pmatrix},e_2 = \begin{pmatrix}0\\1\\0\\...\\0\end{pmatrix},e_1 = \begin{pmatrix}0\\0\\0\\...\\1\end{pmatrix}$$
In $\mathbb{R}^2$, the standard basis vectors are sometimes called $i = e_1$ and $j = e_2$
In $\mathbb{R}^3$, we sometimes use $i = e_1$ and $j = e_2$ and $k = e_3$

<u>Theorem 10.5</u>
A list of vectors $v_1,...,v_n \in V$ is a basis of $V$ if and only if every vector $w \in V$ can be uniquely represented as a linear combination  


# Resources
[[Vector Spaces]]
[[Span and Linear Independence]]
