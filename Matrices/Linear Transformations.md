A <b>function</b> from a set $X$ to a set $Y$, denoted $f: X \to Y$, is  an assignment of a unique value $f(x) \in Y$ to each $x \in X$

The <b>domain</b> of the function is set $X$
The <b>codomain</b> of the function is the set $Y$

Let $V$ and $W$ be vector spaces. The <b>linear transformation</b> (or <b>linear map</b>) from $V$ to $W$ is a function $f: V \to W$ satisfying the following two properties:
	$f$ preserves scalar multiplication if $v \in V$ and $c \in \mathbb{R}$, then $f(cv)=cf(v)$
	$f$ preserves addition if $v,w \in V$,then $f(v+w) = f(v)+f(w)$
The set of all linear transformations from $V$ to $W$ is denoted $L(V,W)$. When $V = W$, this can abbreviated to $L(V)$

<u>Theorem 14.3</u>
If $f: V \to W$ is a linear transformation, then $f(0) = 0$.

<u>Theorem 14.4</u>
Let $f: V \to W$ be a linear transformation, an let $v_1,...,v_n$ be a basis for $V$. The values $f(v_1),...,f(v_n)$ uniquely determine the linear transformation $f$.

<i>Examples of Linear Transformations</i>:
	Scaling
	Rotation about the origin
	Reflection across a line passing through the origin
	Projection onto a line passing through the origin
	Shearing by keeping one direction fixed and tilting another