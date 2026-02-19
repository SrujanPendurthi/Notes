Let $f: V \to W$ be a linear transformation
The <b>kernel</b> of $f$ is the set $\{v \in V| f(v) = 0\}$, denoted $ker(f)$. The kernel of $f$ is a subspace of $V$
The <b>image</b> of $f$ is the set $\{f(v)|v \in V\}$, denoted $im(f)$. The image of $f$ is a subspace of $W$.

Let $f: V \to W$ be linear transformation
$f$ is <b>injective</b>(or <b>one-to-one</b>) if $\forall u,v \in V, \text{if } f(u) = f(v),\text{then } u=v$ 
	That is, every $w \in W$ has at most one $v \in V$ with $f(v) =w$
$f$ is <b>surjective</b>(or <b>onto</b>) if the image of $f$ is all of $W$. 
	That is, every $w \in W$ has at least one $v \in V$ with $f(v) = w$
<u>Theorem 15.3</u>
A linear transformation $f: V \to W$ is injective if and only if $ker(f) = \{0\}$

Let $f: V \to W$ and $g: U \to V$ be linear transformations. The <b>composition</b> $f \circ g: U \to W$ defined by $(f \circ g)(u) = f(g(u)) \forall u \in U$

Let $V$ be a vector space. The <b>identity transformation</b> is the linear transformation $id: V \to V$ defined by $id(v) =v,$ $\forall v \in V$
For any $f \in L(V,W)$, the identity transformation on $V$ satisfies $f \circ id = f$, and the identity transformation on $W$ satisfies $id \circ f = f$
