<b>Equivalence Class of A</b>: $[a] = \{x \in A| x \sim a\}$
<b>Quotient Set</b>: $A/\sim = \{[a]| a \in A\}$
A <b>partition</b> of $A$ is a set of nonempty pairwise disjoint subsets of $A$ whose union is $A$

<i>Example</i>: $A = \{\text{residents of 50 states}\}$, $a \sim b  \iff \text{a and b live in same state}$
	Equivalence Classes $\{AK residents\}, \{AL residents\}, ..., \{WY residents\} \subseteq A$
	Quotient Set: $A/\sim = \{\{AK residents\}, ..., \{WY residents\}\}(\text{This is a partition of A})$

Let ~ be an equivalence relation on a set $A$
	a) $\forall a,b \in A, a \sim b \iff [a] = [b]$
	b) if $a \not\sim b, then [a] \cap [b] = \emptyset$
	Consequently, $A/\sim = \{[a]|a \in A\}$

<u>Proof</u>
$\iff$ Assume $a \sim b$. Show that $[a] = [b]$
	We will use double containment.
	$\to$(Assume $a \sim b$)
		($\subseteq$) Let $x \in [a]$ be arbitrary. Then $x \sim a$ by definition. Since $x \sim a$ and $a \sim b$, by definition of transitivity, $x \sim b$. So, $x \in [b]$. Hence, $[a] \subseteq [b]$
		($\supseteq$)Let $x \in [b]$ be arbitrary. Then, $x \sim b$, by definition. Since $x \sim b$ and $b \sim a$, by definition of transitivity and symmetry, $x \sim a$. So, $x \in [a].$ Hence, $[b] \subseteq [a]$
	$\leftarrow$(Assume $[a] = [b]$)
	Since $\sim$ is reflexive, $a \sim a$. Hence, $a \in [a].$ Since $[a] = [b]$, we have $a \in [b]$. So, $a \sim b$, by definition.
