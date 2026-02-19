<u>Theorem 13.1: Rank-Nullity Theorem</u>
Let $A \in \mathbb{R}^{m \times n}$. Then $rank(A) + dim(N(A)) = n$

<u>Theorem 13.2: Dimensions of Fundamental Subspaces</u>
Let $A \in \mathbb{R}^{m \times n}$ with $r = rank(A)$
	$dim(C(A)) = r$
	$dim(N(A)) = n-r$
	$dim(R(A)) = r$
	$dim(N(A^T)) = m-r$

<u>Theorem 13.3</u>
Let $A \in \mathbb{R}^{m \times n}$ and $B \in \mathbb{R}^{n \times p}$. Then $rank(AB) \le rank(A)$ and $rank(AB) \le rank(B)$.

<u>Theorem 13.4</u>
Let $A \in \mathbb{R}^{m \times n}$. Then:
	Every vector in $R(A)$ is orthogonal to every vector in $N(A)$
	Every vector in $C(A)$ is orthogonal to every vector in $N(A^T)$

<u>Theorem 13.5</u>
Let $A \in \mathbb{R}^{m \times n}$. The only vector in both $R(A)$ and $N(A)$ is 0.

<u>Theorem 13.6</u>
Let $A \in \mathbb{R}^{m \times n}.$ Any vector $x \in \mathbb{R}^n$ can be uniquely written as a sum $x = x_r + x_0$, where $x_r \in R(A)$ and $x_0 \in N(A)$
