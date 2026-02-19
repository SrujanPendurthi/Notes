# Containment and Double Containment Proofs
**Containment Proofs:** To prove $A \subseteq B$:
	Let $a \in A$ be arbitrary
	Show that $a \in B$ 

**Double Containment Proofs:** To prove $A = B$:
	$(\subseteq)$ Let $a \in A.$ Show that $a \in B$.
	$(\supseteq)$ Let $b \in B.$ Show that $b \in A.$ 
# Power Sets
**Definition:** Let $A$ be a set. The power set of $A$, denoted $\mathbb{P}(A)$, is the set of all subsets of $A$. That is,
	$\mathbb{P}(A) = \{B | B \subseteq A\}$ 
For any set $A$, $\emptyset \in \mathbb{P}(A) and A \in \mathbb{P}(A)$ 


# Fundamental Set Operations
$U$ is the universal set

**Pairwise Intersection**, denoted $A \cap B$, returns the sets of all elements that $A$ and $B$ have in common. 
$A \cap B = \{x \in U | x \in A \wedge x \in B\}$ 

**Pairwise Union**, denoted $A \cup B$, returns the set of all elements of $A$ and $B$

Associative and Commutative properties hold, same as logical operators

**Set Difference**, denoted $A \setminus B$, returns the set of all elements that are present in $A$, but not in $B$

$A \setminus B = \{x \in U | x \in A \wedge x \notin B\}$

**Complement**, denoted $A^c$, is the set of all elements in $U$ that are not in $A$.
	$A^c = \{x \in U | x \notin A\} = U \setminus A$ 

**Disjoint** if $A \cap B = \emptyset$ 
# **Indexed Unions and Intersections**
Indexing sets is useful when we want to define or reference a large number of sets without listing each one explicitly

**Definition:** Let $I$ be a set. A *family of sets indexed by* $I$, or simply and *indexed family of sets,* is a collection where each element of $I$ corresponds to a set $A_i$. The set $I$ is called an *index set*. We typically denote the indexed family of sets as either $\{A_i | i \in I\}$ or $\{A_i\}_{i \in I}$. 

**Definition:** Let $\{A_i\}_{i \in I}$ be an indexed family of sets. We define:
	**Indexed Intersection:** $$\bigcap_{i\in I}A_i = \{x \in U | \forall i \in I, x \in A_i\}$$
	**Indexed Union:**
	$$\bigcup_{i \in I}A_i = \{x \in U | \exists i \in I, x \in A_i\}$$

**DeMorgan's Laws for Sets**
	If $A,X,Y$ are sets, then
		$A \setminus (X \cup Y) = (A \setminus X) \cap (A \setminus Y)$ 
		$A \setminus (X \cap Y) = (A \setminus X) \cup (A \setminus Y)$ 
	Additionally, let ${X_i | i \in I}$ be an indexed family of sets. Then
		$A \setminus \bigcup_{i \in I}X_i = \bigcap_{i \in I}(A \setminus X_i)$
		$A \setminus \bigcap_{i \in I}X_i = \bigcup_{i \in I}(A \setminus X_i)$

$\bar{A \cap B} = \bar{A} \cup \bar{B}$
$\bar{A \cap B} = \bar{A} \cap \bar{B}$

# **Cartesian Products**
The Cartesian Product of two sets provides a way to pair each element of one set with each element of another set.
	Allows us to construct ordered pairs and define relationships and functions
	**Definitions:** Let $A$ and $B$ be sets. The Cartesian product of $A$and $B$, denoted $A \times B$ is defined as follows:
		$A \times B = \{(a,b)|a \in A \wedge b \in B\}$
	where the elements $(a,b) \in A \times B$ are *ordered pairs*.
	The defining property of an ordered pair is that for $a,c \in A$ and $b,d \in B$
		$(a,b) = (c,d)$ if and only if $a=c$ and $c = d$ 
	**Repeated Cartesian Products:** $A \times (B \times C) \equiv A \times B \times C$ 

**Set Equality via Logical Equivalences**
	Set equality can be viewed as a biconditional statement
	$A = B  \to (\forall x \in U, (x \in A \iff x \in B))$ 
	For any sets $A, B, \text{ and } C,$ we have
		$C \subseteq A \cap B \iff C \subseteq A \wedge C \subseteq B$
	For all sets $A$ and $B$,
		$\mathbb{P}(A) \cap \mathbb{P}(B) = \mathbb{P}(A \cap B)$
	**Proving Set Equality via Logical Equivalences**:
		To prove $A = B$
			1. Let $U$ be a universal set containing both $A$ and $B$
			2. Translate the statement $A = B$ into logical form
			3. Fix an arbitrary element $x$ in the universal set under consideration
			4. Build a chain of equivalences, starting from $x \in A$ and step by step transforming it into $x \in B$, using only definitions, algebraic manipulations, and previously proven biconditionals
			5. Conclude that $x \in A \iff X \in B$ holds for all x, and therefor $A = B$

# Resources
[[Proof Strategies]]