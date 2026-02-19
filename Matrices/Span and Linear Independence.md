
A <b>linear combination</b> of $v_1,v_2,...,v_3$ is a vector of the form $$c_1v_1 + c_2v_2 + ... + c_nv_n$$for some scalars $\in \mathbb{R}$

The <b>span</b> of a list of vectors is the set of all linear combinations of those vector
	By convention, the span of an empty list of vectors is the set {0}
	$$span(v_1,v_2,..,v_n) = \{c_1v_1 + c_2v_2 + ...+ c_nv_n\}$$
The span represents all reachable points of a vector whereas the linear combination of a vector represents a single vector

<u>Theorem 9.2</u>
Let $v_1,...v_n$ be vectors in a vector space $V$. Then span($v_1,...,v_n$) is a subspace of $V$

# Linear Independence
A list of vectors $v_1,v_2,...v_n$ is <b>linearly independent</b> if the only solution to the equation $c_1v_1 + c_2v_2 + ...+ c_nv_n = 0$ is the trivial solution. If there are any other solutions, then the vectors are <b>linearly dependent</b>
	We can easily figure out if a set of vectors is linearly independent by using an augmented matrix with the right side being 0's and doing the RREF. If there are free variables then it is linearly dependent
	Or you could show that the linear combination of each vector has only the trivial solution
Think of linear combinations are for one vector and RREF method is for a list of vectors


# Resources
[[Linear Systems and RREF]]
[[Introduction and Vector Operations]]
