# Existential Statements
Indirect Proof Strategy: Assume for the sake of contradiction(AFSOC) that $\forall x \in S, \neg P(x) \text{ holds}$. Derive a contradiction from this assumption. Conclude that $\exists x \in S, P(x)$ must be true.

**Floor**, denoted $\lfloor x\rfloor$, is the function that returns greatest integer, $n$, such that $n \le x$.
**Ceiling**, denoted $\lceil x \rceil$, is the function that returns the least integer, $n$, such that $n \ge x$.

**Pigeonhole Principle:** Let $n,k \in \mathbb{Z}^+$. If $n$ objects are placed into $k$ boxes, then there exists a box containing at least $\lceil \frac{n}{k} \rceil$ objects.
	Proof: Suppose objects $a_1,a_2,...,a_n$, are placed into boxes $A_1,A_2,...,A_3$. Assume for the sake of contradiction that
		$\forall i \in [k], A_i \text{ contains fewer than } \lceil \frac {n}{k} \rceil \text{ objects.}$
		Since each $A_i$ contains an integer number of objects, this means
		$\forall i \in [k], A_i \text{ contains at most } \lceil \frac {n}{k} \rceil -1 \text{ objects}.$ 
		By definition of the ceiling function, we have
		$\lceil \frac {n}{k} \rceil -1 < \frac {n}{k} \le \lceil \frac{n}{k} \rceil$ 
		Therefore, the total number of objects in all $k$ boxes is at most
		$k * (\lceil \frac{n}{k} \rceil - 1) < k * \frac {n}{k} = n,$ 
		contradicting the fact that exactly $n$ objects were placed into the boxes.
		Hence, there must exist some $i \in [k]$ such that $A_i$ contains at least $\lceil \frac{n} {k} \rceil$ objects.
# Conditional Statements
Conditional statements are those in the form $P \to Q$.

Proofs of Conditional Statements are the most common in mathematics.

**Direct Proof Strategy:** Assume $P$ is true. Show that $Q$ must also be true.


**Indirect Proofs Strategies:**
	**Contrapositive Proof Strategy:** Assume $\neg Q$ is true. Show that $\neg P$ must also be true
	**Contradiction Proof Strategy:** Assume for the sake of contradiction that $P \wedge \neg Q$ holds. Find a contradiction based on this assumption. Conclude that $P \to Q$ must hold

# Biconditional Statements
There are two common techniques for proving biconditional statements
	Standard Method
	Intermediary Method

**Standard Method:** Provide both directions separately:
	Assume $P$ and show $Q$ 
	Assume $Q$ and show $P$ 

 **Intermediary Method:** Construct a sequence of reversible logical steps:
	 $P \iff A \iff B \iff ... \iff Q$
	Creating a chain of logical equivalences in which each step is reversible can be challenging
	Most effective for simpler propositions where each step is justified

Notes about Disjunctions:
	To prove $(P \lor Q) \to R$ directly, break into cases:
		Case 1: Assume $P$ holds. Prove $R$ holds.
		Case 2: Assume $Q$ holds, Prove $R$ holds.
	If the two cases are symmetrical, we may use the "without loss of generality" (WLOG)
	To prove $P \to (Q \lor R):$
		Direct Proof: Assume $P \wedge \neg Q.$ Prove $R$ 
		Indirect Proof: Use contrapositive: assume $\neg Q$ and $\neg R$, to prove $\neg P$
# Existence and Uniqueness Proofs
Propositions of the form $\exists ! x \in S, P(x)$ 
	**Existence:** Prove the existential statement $\exists x \in S, P(x)$ using established methods
	**Uniqueness:** Let $x,y \in S$ such that $P(x)$ and $P(y)$ both hold. Show that $x = y$ 
# Proof-Writing Tips
Writing Proofs:
	Central Tips:
		State Your Hypotheses
		Include All Steps
		Explain Why Steps are Valid
	Syntax Tips:
		Define New Variables or Notation
		Use First Person Plural
		Use Complete Sentences
		Indicate Directions in Biconditional Proofs
		Use Appropriate Notation
	Revision Tips:
		Revise and Refine
		Check Your Proof's Structure

Coming up with Proofs:
	Determine Hypotheses
	Clarify the Goal
	Use Scratch Work
	Look for Similar Proofs
	Check Definitions
	Use Concrete Examples
	Search for Counterexamples
	Proceed by Contradictions

Common Mistakes:
	Avoid Variable Duplication
	Understand Definitions

General Advice:
	Practice Regularly
	Incorporate Feedback
	Work on Proof Readability
	Understand Presented Proofs
	Do not Rely Solely on Posted Solutions

Writing Proofs is just expressing logic in the context of writing about math, learn more in [[Logic]]

