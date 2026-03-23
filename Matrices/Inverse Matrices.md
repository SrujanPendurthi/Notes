The <b>inverse</b> of a square matrix $A \in \mathbb{R}^{m \times n}$ is the matrix $A^{-1}$ satisfying $AA^{-1} = I_n$ and $A^{-1}A = I_n$.

A square matrix is called <b>invertible</b> if it has an inverse and singular if it does not have an inverse

Not every matrix has an inverse.

If $f: V \to W$ is an invertible linear transformation with matrix $A$, then the matrix for $f^{-1}$ is $A^{-1}$

In order to find the inverse of a square matrix, we can use Gauss-Jordan Elimination
	Start with $[A|I_n]$, then get it into RREF, which should give you $[I_n|A^{-1}]$. Otherwise, $A$ has no inverse

<u>Theorem 18.3: Inverse of a 2 x 2 Matrix</u>
The inverse of a $2 \times 2$ matrix $A$ = $\begin{pmatrix}a & b \\ c & d\end{pmatrix}$ is $A^{-1} = \frac{1}{ad-bc}\begin{pmatrix}d & -b \\ -c & a\end{pmatrix}$. The inverse exists if and only if $ad -b \ne 0$

<u>Theorem 18.4</u>
The inverse of an invertible matrix is unique

<u>Theorem 18.5</u>
Let $A,B \in \mathbb{R}^{n \times m}$. Then $AB = I_n$ if and only if $BA = I_n$.

<u>Theorem 18.6: Invertible Matrix Theorem</u>
Let A be an n × n real matrix. The following are equivalent:
	(a) The inverse A−1 exists.
	(b) The RREF of A is In.
	(c) rank(A) = n.
	(d) The equation Ax = b has a unique solution for any b ∈ Rn.
	(e) N (A) = {0}.
	(f) dim(N (A)) = 0.
	(g) The columns of A are linearly independent.
	(h) The columns of A form a basis for Rn.
	(i) C(A) = Rn.
	(j) dim(C(A)) = n.
	(k) A⊤ is invertible.
	(l) N (A⊤) = {0}.
	(m) dim(N (A⊤)) = 0.
	(n) The rows of A are linearly independent.
	(o) The rows of A form a basis for Rn.
	(p) R(A) = Rn.
	(q) dim(R(A)) = n.
	(r) The linear transformation f : Rn → Rn with f (v) = Av is injective.
	(s) The linear transformation f : Rn → Rn with f (v) = Av is surjective.
	(t) The linear transformation f : Rn → Rn with f (v) = Av is an isomorphism.
Note: “Equivalent” means that if any one of these statements is true, then they’re all true, and if
any one of these statements is false, then they’re all false