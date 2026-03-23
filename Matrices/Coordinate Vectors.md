Let $V$ be a vector space and $\beta$ be a basis $v_1,...,v_n$ of $V$. For a vector $v \in V$, the <b>coordinate vector</b> of v in the basis $\beta$ is:
	$$[v]_\beta = \begin{pmatrix}c_1 \\...\\c_n\end{pmatrix}$$, where $v = c_1v_1 + ...+ c_nv_n$ 
The standard basis $e_1,...,e_n$ of $\mathbb{R}^n$ denoted $\epsilon$. if $v$ is a vector in $\mathbb{R}^n$, then $[v]_\epsilon = v$

Let $V$ be a n-dimensional vector space with basis $\alpha$ and $\beta$. The <b>change of basis matrix</b> from $\alpha$ to $\beta$ is the $n \times n$ matrix $P$ such that $[v]_\beta = P[v]_\alpha$ for all $v \in V$. The columns of $P$ are the vectors $[v_1]_\beta,...,[v_n]_\beta,$ where $\alpha = \{v_1,...,v_n\}$. The change of basis matrix from $\beta$ to $\alpha$ is $P^{-1}$ 

Let $A$ and $B$ be $n \times n$ matrices. We say that $A$ is similar to $B$ if there is a matrix $P \in \mathbb{R}^{n \times n}$ such that $A = PBP^{-1}$ or $B = P^{-1}AP$ 

<u>Theorem 19.4</u>
Let $V$ be an n-dimensional vector space with bases $\alpha$ and $\beta$. Suppose $f: V \to V$ is a linear transformation where $A$ is the matrix of $f$ in basis $\alpha$ and $\beta$ is the matrix of $f$ in basis $\beta$. Then $A = PBP^{-1}$, where $P$ is the change of basis matrix from $\beta$ to $\alpha$ 

# Resources
[[Linear Independence and Bases]]