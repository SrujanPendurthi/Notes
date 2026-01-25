Properties of Matrix Multiplication
	Associative: $A(BC) = (AB)C$
	Distributive: $A(B+C) = AB + AC$
	NO Commutative Property(not always true)
		$AB \ne BA$

Transpose
	Operation done to a single matrix
	Suppose $A$ is an $m * n$ matrix. $A^T$ is the $n *m$ matrix with the rows of A written vertically as columns
	That is, if $A = [a_{ij}], A^T = [a_{ji}]$
	$(AB)^T = (B^TA^T)$
Let $\vec{v}, \vec{w} \in \mathbb{R}^n$ be column vectors
	*Inner Product*: the scalar $\vec{v}^T * \vec{w}$
		(same as the dot product of $\vec{v} \cdot \vec{w}$)
	*Outer Product*: the $n * m$ matrix $\vec{v}\vec{w}^T$
		$(n * 1)(1 * n) \to (n * n)$

Cannot always cancel out terms with matrices

**Identity** Matrix
	 the $n *n$ matrix $I_n$ with entries $I_ij = \{1 \text{ if } i =j, 0 \text{ if } i \ne\}$
	 We have $AI_n = A$ and $BI_n$ = B  for any matrices $A \in \mathbb{R}^{n * p}$  and $B \in \mathbb{R}^{n*p}$ 
	 The identity matrix is the "I" of matrices

**Inverse Matrix**
	The inverse of a square matrix $A \in \mathbb{R}^{n*n}$ is the $n*n$ matrix $A^{-1}$ satisfying $AA^{-1} = I_n$ and $A^{-1}A = I_n$
	A matrix is *invertible* if it has an inverse and *singular* if it does not

