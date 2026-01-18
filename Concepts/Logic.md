# Propositional Logic
In propositional logic, we examine the logical relationships between various mathematical statements based on their sentence structure

**Atomic Proposition(or atom)** is a proposition whose truth value is independent of the truth value of any other proposition. 
	In particular, an atomic proposition CANNOT be broken down into simpler propositions

We can use propositional variables to denotes atomic propositions, using the := operator 

**Conjunction**, denoted $\wedge$, is when any two propositions can be combined to form a new proposition
	Translated as "and"
	$P \wedge Q$ is true if and only if other $P$ and $Q$ are true
	
	
| $P$ | $Q$ | $P\wedge Q$ |
| --- | --- | ----------- |
| T   | T   | T           |
| T   | F   | F           |
| F   | T   | F           |
| F   | F   | F           |

**Disjunction**, denoted $\lor$, is when any two propositions can be combined to form a new proposition
	Translated as "or"
	$P \lor Q$ is true if and only if either $P$ is true or $Q$ is true or both
		

| $P$ | $Q$ | $P \lor Q$ |
| --- | --- | ---------- |
| T   | T   | T          |
| T   | F   | T          |
| F   | T   | T          |
| F   | F   | F          |
**Negation**, denoted $\neg$ is when we form a new proposition given a single proposition
	Translated as "not"
	$\neg P$ is true if and only if $P$ is false
	 

| $P$ | $\neg P$ |
| --- | -------- |
| T   | F        |
| F   | T        |
**Logical Implication**, denoted $\to$,  is translated "if $P$ then $Q$"
	Does not implicate causuality
	$P$ is known as the antecedent, hypothesis, or supposition
	$Q$ is the consequent or conclusion
	*Modus Ponens* is deducing $Q$ is true when $P \to Q$ is true and $P$ is true
	As seen in the truth table, when the antecedent is `False`, the conclusion is always `True`. This is something called *Vacuously True*. Since the entire premise is `False`, there are no cases to check, making the statement `True` by default. However, this is pretty empty and useless

| $P$ | $Q$ | $P \to Q$ |
| --- | --- | --------- |
| T   | T   | T         |
| T   | F   | F         |
| F   | T   | T         |
| F   | F   | T         |
**Biconditional Connective**, denoted $\iff$, is translated "$P$ if and only if $Q$" 
	This means for $P$ to be `True` ($P \to Q \wedge Q \to P$) must be `True` 
	If $P \iff Q$ is `True` for all possible truth values of the atomic propositions, then we says $P \equiv Q$ or $P$ and $Q$ are *logically equivalent*
	A biconditional is the implication+ the converse of the implication

| $P$ | $Q$ | $P\iff Q$ |
| --- | --- | --------- |
| T   | T   | T         |
| T   | F   | F         |
| F   | T   | F         |
| F   | F   | T         |
A **tautology** is when a propositional formula is always `True`
A **contradiction** is when a propositional formula is always `False`
## Logical Equivalences
**De Morgan's Law for Connectives:** For all propositions $P$ and $Q$, the following logical equivalences hold `True`:
	$\neg (P \wedge Q) \equiv (\neg P \lor \neg Q)$ 
	$\neg(P \lor Q) \equiv (\neg P \wedge \neg Q)$ 

**Distributive Law for Connectives:** For all propositions $P, Q \text{ and } R$, the following logical equivalences hold:
	$P \wedge (Q \lor R) \equiv (P \wedge Q) \lor (P \wedge R)$ 
	$P \lor (Q \wedge R) \equiv (P \lor Q) \wedge (P \lor R)$ 

**Law of Double Negatives:** For any proposition $P$, $\neg \neg P \equiv P$

**Associative Law:** For any proposition $P,Q, R$, the following are true:
	$P \wedge (Q \lor R) \equiv (P \wedge Q) \lor (P \wedge R)$
	$P \lor (Q \wedge R) \equiv (P \lor Q) \wedge (P \lor R)$
	This means we can basically get rid of parentheses, but only when there are the same type of junctions(need parentheses for a statement with both disjunctions and conjunctions):
		$P \lor (Q \lor R) \equiv P \lor Q \lor R$

**Commutative Law:** For any proposition $P \text{ and } Q$, the following are true:
	$P \wedge Q \equiv Q \wedge P$
	$P \lor Q \equiv Q \lor P$
**Biconditional Equivalence:** For any proposition $P \text{ and } Q$,
	$P \iff Q \equiv (P \to Q) \wedge (Q \to P)$

**Disjunctive Form of Implication:** For any proposition $P \text{ and } Q$,
	$P \to Q \equiv \neg P \lor Q$


**Contrapositive:** For any proposition $P \text{ and } Q$, 
	$P \to Q \equiv \neg Q \to \neg P$

# Predicate Logic
**Predicate** is a statement involving free(unbound) variables. 
	AKA variable proposition
	A predicate itself does not have a truth value, but it takes a truth value once its variables are specified
	*Examples: $P(x) := x^2 \ge 8$* defined on $x \in \mathbb{R}$
		The truth value of the predicate above depends on the value of x, a variable

One way to turn a predicate into a proposition is to specify how often the predicate holds `True`. We do this using *quantifiers*.

**The Universal Quantifier**, denoted $\forall$, translates to "for all."

**The Existential Quantifier**, denoted $\exists$, translates to "there exists."

*Quantifier + Proposition = Predicate*

**Maximally Negating Propositions** is negating every atomic formula.
	It is often useful in order to understand a statement deeper, specifically when writing a proof by contradiction.

**DeMorgan's Laws for Quantifiers:** For any set $S$ and predicate $P(x)$:
	$\neg \forall \in S, P(x) \equiv \exists x \in S, \neg P(x)$
	$\neg \exists x \in S, P(x) \equiv \forall x \in S, \neg P(x)$

Statements that involve quantifiers, truth tables cannot be used to establish the equivalences

Finding a Maximally Negated Form:
	*Move negations inward* - Start with the outermost negation and apply rules for negating quantifiers
	*Push negations through connectives* - Use DeMorgan's Laws and double negation elimination
	*Rewrite Implications* - Replace $A \to B$ with $\neg A \lor B$ before pushing negations inside
	*Repeat until only atomic formulas are negated* - Continue applying the rules unit no quantifiers or connectives have a negation directly in front of them
# Converse, Inverse, Contrapositive
A **Contrapositive** of a conditional statement,$p\to q$, is $\neg q \to \neg p$, making a logically equivalent statement

A **Converse** of a conditional statement, $p \to q$, is $q \to p$, making them not always logically equivalent

An **Inverse** of a conditional statement, $p \to q$, is $\neg p \to \neg q$, making them not always logically equivalent

Since the original and contrapositive are logically equivalent, it makes them very powerful tools in certain proof writing strategies

The Inverse and Converse are logically equivalent

# Proof Writing
**Direct Proofs** are proofs that attempt to establish the truth of the statement as written 

**Indirect Proofs** are proofs that establish the truth of a logically equivalent statement

A **Universal Statement** is a proposition of the form $\forall x \in S, P(x)$
	**Direct Proof Strategy:** Let $x \in S$ be arbitrary but fixed. Demonstrate that $P(x)$ is true. Since $x \in S$ was chosen arbitrarily, we may conclude that $\forall x \in S, P(x)$ is true.
		*Containment Proofs* are when we need to proof $A \subseteq B \iff \forall a \in A, (a \in B)$. We do this by letting $a \in A$ be arbitrary and then show that $a \in B$.
	**Indirect Proof Strategy:** To prove $\forall x \in S, P(x)$ indirectly, assume for the sake of contradiction(AFSOC) that $\exists x \in S, \neg P(x) \text{ holds}$. Fix such an $x$ and proceed through a chain of logical deductions until you arrive at a contradiction. Conclude that $\forall x \in S, P(x)$ must be true. 
An **Existential Statement** is a proposition of the form $\exists x \in S, P(x)$ 
	**Direct Proof Strategy:** Demonstrate that there exists $x \in S$ such that $P(x)$ holds
	Proof by demonstration is the most common approach, where we provide a concrete example or counterexample
A **constructive proof** proves a mathematical statement, especially an existence claim (e.g., "there exists an X such that..."), by explicitly providing the object or an algorithm to create it.
	This method builds the object directly, making it demonstrable and often algorithmic, contrasting with classical logic's reliance on indirect methods like proof by contradiction which might rely on the law of the excluded middle
Unlike **non-constructive proofs** which show an object must exist without showing how to find it

# Resources
https://www.youtube.com/watch?v=A3Ffwsnad0k&list=PLl-gb0E4MII28GykmtuBXNUNoej-vY5Rz