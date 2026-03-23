Let $f: A \to B$
$f$ is <b>surjective</b>(onto) if $\forall b \in B, \exists a \in A, b = f(a)$
	every $b \in B$ has a preimage or $f[a] = B$
$f$ is <b>injective</b>(one-to-one) if 
	$\forall a_1, a_2 \in A, a_1 \ne a_2 \to f(a_1) \ne f(a_2)$
	$\forall a_1,a_2 \in A, f(a_1) = f(a_2) \to a_1 = a_2$ (this is the contrapostive of the above condition)
	every $b \in f[A]$ has a unique preimage
$f$ is a <b>bijection</b> if $f$ is injective and surjective

The <b>identity function</b> $i_A: A \to A$ is defined by $i_A(a)=a$ for all $a \in A$ is a bijection

# Proof Strategies
In order to prove $f$ is injective
	Direct: Assume $a_1 \ne a_2$, Prove $f(a_1) \ne f(a_2)$
	Contrapositive: Assume $f(a_1) = f(a_2)$. Show $a_1 = a_2$

In order to prove $f$ is not injecive:
	Counterexample: Find $a_1,a_2$ such that $a_1 \ne a_2$ and $f(a_1) = f(a_2)$

In order to prove $f$ is surjective:
	Choose an arbitrary $b \in B$. Find $a \in A$ such that $f(a) =b$

In order to prove $f$ is not surjective:
	Counterexample: Find $b \in B$ such that $f(a) \ne b, \forall a \in A$

# Function Equality
Let $f: A \to B$ and $g: A \to D$ be functions. Then $f$ and $g$ are equal if they are equal as sets.
	This means you must translate both functions into set-builder notation, then do a double containment

# Resources
[[Functions]]
[[Sets]]
[[Disproof Strategies]]
[[Proof Strategies]]
