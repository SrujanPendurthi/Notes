<u>Theorem 16.1: Matrix of a Linear Transformation(for real vectors)</u>
Let $f: \mathbb{R}^n \to \mathbb{R}$ be a linear transformation. There exists a matrix $A \in \mathbb{R}^{m \times n}$ such that $f(v) = Av$ for all $v \in V$. The columns of $A$ are $f(e_1),...,f(e_n)$, where $e_1,...,e_n$ is the standard basis of $\mathbb{R}^n$

<u>Theorem 16.2: Matrix of a Linear Transformation(general form)</u>
Let $f: V \to W$ be a linear transformation. Suppose $v_1,...,v_n$ is a basis for $W$. Then, there exists a matrix $A \in \mathbb{R}^{m \times n}$ such that $f(v) = Av$ for all $v \in V$(represented as real vectors). The columns of $A$ are $f(v_1),...,f(v_n)$(represented as real vectors)

<u>Theorem 16.3: Linear Transformations are Matrices</u>
Let $f: V \to W$ be a linear transformation that has matrix $A \in \mathbb{R}^{m \times n}$ with respect to some bases for $V$ and $W$, where $n = dim(V)$ and $m = dim(W)$. By representing vectors in $V$ and $W$ as real vectors, we have the following relationships between linear transformation $f$ and its matrix $A$
	The kernel of $f$ is the null space of $A$
		$ker(f)$ is the set of vectors $v \in V$ such that $f(v) = 0$ and $N(A)$ is the set of vectors $Av = 0$. Since $f(v) =Av$, the two sets are the same
	The image of $f$ is the column space of $A$.
		$im(f)$ is the set of vectors $f(v)$ where $v \in V$. $C(A)$ is the set of vectors $Av$ where $v \in \mathbb{R}^n$. As $f(v) =Av$, these sets are the same, except vectors are represented as real vectors in $C(A)$
	By the rank-nullity theorem, $dim(im(f)) + dim(ker(f)) = n$
		Because you can written the rank nullity theorem like $dim(C(A)) + dim(N(A))= n$
	$f$ is injective if and only if $N(A) = \{0\}$
	$f$ is surjective if and only if $C(A) = \mathbb{R}^n$
	If $g: U \to V$ is a linear transformation with matrix $B$, the matrix for the composition $f \circ g$ is the product $AB$
		Since $f(v) = Av$ and $g(u) = Bu$, we have $f(g(u)) = ABu = (AB)u$, so the matrix of $f \circ g$ is $AB$
	The identity transformation $id: V \to V$ has the matrix $I_n$
		The identity transformation is $f(v) = v$, so its matrix should also satisfy $Av = v$ whenever $v$ is a real vector. This is true for the matrix $A = I_n$