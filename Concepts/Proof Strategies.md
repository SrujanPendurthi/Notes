Basic Proof Strategies
A mathematical statement has an assumption A and a consequence C
When $P \to Q$, we assume $P$, then prove $Q$.

Direct Proof:
	Derive a string of simple implications from A to C.
	$A \to A_1  \to A_2 \to ... \to A_k \to C$
	Prove if $A$, then $C$ 

Definition of even: An integer $n$ is even if $n = 2k$ for some $k \in \mathbb{Z}$
Definition of odd: An integer $n$ is even if $n = 2k + 1$ for some $k \in \mathbb{Z}$

Proof by Cases:
If $A$ is of the form $p_1 \lor p_2 \lor ... \lor p_n$, we can break $(p_1v...vp_n) \to C$ into cases:
	$p_1 \to C_1$, $p_2 \to C$, $p_n \to C$  
	Prove if $A_1$ then C. We can break $A$ into the cases $p_1,...,p_n$. We will prove $C$ in each of the cases.
		Case 1: $p_1 \to C$
		Case n: $p_n \to C$

Proof by Contrapositive:
Instead of proving $A \to C$, prove $\neg C \to \neg A$, which we know is logiclaly equivalent to $A \to C$ 
Prove if A, then C. Assume $\neg C$, prove $\neg A$ 


Proof by Contradiction:
Prove if $A$, then $C$,
Proof: Assume $A$, then $C$,
	For the sake of contradiction, assume $\neg C$
	Then $B$, which is a false statement.
	Hence, our assumption $\neg C$ is False. Thus, $C$ is True

example:
	Prove that there is no largest integer.
		Proof: For the sake of contradiction,
		Assume there is a largest integer, $N$
		Then $N+1 \le N$, which is absurd.
		So out assumption was wrong. Hence there is no largest integer
	So we assumed the negation of the statement, then shows that the negation was False in order to show the original statement was True

# Resources
[[Logic]]