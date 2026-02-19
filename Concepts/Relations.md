A <b>binary relation</b> on $A$ is a subset of $A\times A$
<u>Notation</u>: We denote $(x,y) \in R$ by $xRy$ ($x$ is related to $y$)

A binary relation on $A$ is <b>reflexive</b> if $\forall x \in A, xRx$ 
	In order to <i>prove</i> reflexivity, we need to do a general proof using an arbitrary value because it is a universal statement
	In order to <i>disprove</i> reflexivity, we just need a counterexample because we are disproving a universal statement
	<u>Example</u>: Let $A = R$
			$R = \{(x,y)\in \mathbb{R}^2| x \le y\}$ is reflexive. Let $x \in \mathbb{R}$. Then $x \le x$. So $xRx$. Therefore, $R$ is reflexive

A binary relation on $A$ is <b>symmetric</b> if $\forall x,y \in A, xRy \to yRx$
	To <i>disprove</i>, you only need a counterexample because it is a universal statement
	To <i>prove</i>, you need to use an arbitrary value because it is a universal statement			
	<u>Example</u>: Let $A = R$
			$R = \{(x,y)\in \mathbb{R}^2| x \le y\}$ is not symmetric. Since $0 \le 1$, $(0,1) \in R$. But, since $1 \ngeq 0$, so $(1,0) \notin R$
	<u>Example:</u> $R = \{(x,y) \in \mathbb{Z}^2 | x-y \text{ is even}\}$
			Let $x,y \in \mathbb{Z}$ such that $xRy$. Then $x-y = 2k$ for some $k \in \mathbb{Z}$. Now, $y-x = -(x-y) = -2k = 2(-k)$. Since $-k \in \mathbb{Z}$, $y - x$ is even. Hence, $yRx$
 
 A binary relation on $A$ is <b>transitive</b> if $\forall x,y,z \in A, xRy \land yRz \to xRz$ 
	 To <i>disprove</i>, find a counterexample($x,y,z$) that satisfies $xRy,yRz$, but not $xRz$
	 To <i>prove</i>, you need to use an arbitrary value because it is a universal statement
	 <u>Example</u>: $R = \{(x,y) \in \mathbb{R}^2 | y = x^2\}$
			 Since $2^2 = 4$, $(2,4) \in R$. Since $4^2 = 16, (4,16) \in R$.
			 But since $2^2 \ne 16,(2,16) \notin R$  

A binary relation on $A$ is <i>antisymmetric</i> if $\forall a,b \in A, aRb \land bRa \to a = b$ 
	Does not mean not symmetric
	Cannot have unique elements satisfying $aRb$ ans $bRa$
	To <i>disprove</i>, you only need a counterexample because it is a universal statement
	To <i>prove</i>, you need to use an arbitrary value because it is a universal statement

A binary relation $R$ on a set $A$ is called an <b>equivalence relation</b> if $R$ is reflexive, symmetric, and transitive
<u>Notation</u>: In this case, $xRy$ by $x~y$