Two sets $A$ and $B$ have the same cardinality if there is a bijection $f: A \to B$ 

Example: $\{1,2,3\}$ and $\{a,b,c\}$ have the same cardinality since the function $f: {1,2,3} \to {a,b,c}$ given by $f(1) =a,f(2)=b,f(3)=c$ is a bijection
 
Natural numbers and Integers have the same cardinality since $f: \mathbb{N} \to \mathbb{Z}$ by $f(n) = n/2$ when n is even and $f(n) = -(n+1)/2$ if n is odd

For any integer $n \ge 0$,define $[n] = \{k \in \mathbb{Z}| 1 \le k \le n\}$
	$[3] = \{1,2,3\}$, $[0] = \emptyset$,

<u>Lemma:</u> Let $f: [n] \to [m]$ be a function
	a) if $f$ is injective, then $n \le m$
	b) if $f$ is surjective, then $n \ge m$ 
	<i>Proof</i>: We will use weak induction on $n$ to prove: $\forall n \in \mathbb{N}$, if $f: [n] \to [m]$ is injective for some $m \in \mathbb{N}$, then $n \le m$
		Base Case: Let $f: [0] \to [m]$ is injective for some $m \in \mathbb{N}$. Since $m \in \mathbb{N}, 0 \le m$ by default.
		Induction Step: Let $k \ge 0$ and is injective for some $m \in \mathbb{N}$ if $f:[k] \to [m]$ is injective, then $k \le m$. Now let $f: [k+1] \to [m]$ be injective for some $m \in \mathbb{N}$. 
		Define $g: [k+1] \setminus \{k+1\} \to [m] \setminus \{f(k+1)\}$ by $g(x) = f(x)$ for all $1 \le x \le k$ . Since $f$ is injective, so is $g$
		Define $h: [m] \setminus \{f(k+1)\} \to [m-1]$ by $h(x)=\begin{cases}x \text{ if }1 \le x < f(k+1) \\ x-1 \text{ if }f(k+1) < x \le m \end{cases}$
		Then $h$ is injective. Hence $h \circ g: [k+1] \setminus \{k+1\} = [k] \to [m-1]$ is injective.
		Using Inductive Hypothesis, $k \le m -1$. So $k+1 \le m$. By weak induction, $\forall n \in \mathbb{N}$, if $f: [n] \to [m]$ is injective, then $n \le m$

<u>Corollary:</u> $[n] \text{ and } [m]$ have the same cardinality if and only if $n = m$
Proof: 
	Assume $[n]$ and $[m]$ have the same cardinality. Then there is a bijection $f: [n] \to [m]$. Since $f$ is injective, $n \le m$. Since $f$ is surjective, $n \ge m$. Hence, $n =m$
	Assume $n =m$. Then $[n]=[m]$. Since $i_[m]:[m] \to [m]=[n]$ is a bijection, $[n]$ and $[m]$ have same cardinality

$A$ is finite if there is a bijection $f: [n] \to A$ for some $n \in \mathbb{N}$. 
	Example: $\{a,b,c\}$ is finite since $f:[3] \to \{a,b,c\}$ given $f(1) =a,f(2)=b,f(3)=c$ is a bijection. 

