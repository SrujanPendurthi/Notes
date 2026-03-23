# Weak Induction
# Strong Induction
Only differences between strong and weak induction is the assumption or the induction hypothesis and number of base cases

The induction hypothesis has a stronger assumption.
	Instead of assuming $P(k)$, strong induction assumes for all of $n$ smaller than $k$ 

Usually, we use multiple base cases, when there it a recursively defined

Example: Proving that all integers $n \ge 2$ are product of primes using Strong Induction.
	Base Case:
		Since 2 is prime, the statement is true when $n = 2$
	Induction Step:
		Let $k \ge 2$ be an integer and assume that every integer $n$ such that $2 \le n \le k$, $n$ is prime or a product of primes
	Case 1: If $k + 1$ is prime, then we are done
	Case 2:
		Assume $k +1$ is not prime, then $k+1 = ab$ for some $a,b \in \mathbb{N}$ such that $1 < b < k+1$
		Since $2 \ge a \ge k$ and $2 \ge b \ge k$, using the induction hypothesis, $a$ and $b$ are prime or products of primes. Hence, $k +1 = ab$ is a product of primes.
	By Strong Induction, $\forall n \ge 2,n$ is prime or a product of primes. $\square$   

Example: Define the sequence $a_0,a_1,a_2,...$ recursively by $a_0 = 1$, $a_1 = 2$, $a_n= 5{a_{n-1}}-6a_{n-2}$  $\forall n \ge 2$. Prove $a_n = 2^n$ $\forall n \ge 0$.
	Bases Cases: Since $a_0 = 1$ and $2^0 = 1$, so $a_0 = 2^0$. Since $a_1 = 2$ and $2^1 = 2$, so $a_1 = 2^1$. So $a_n = 2^n$ for $n = 0,1$ 
	Induction Step: Let $k \ge 2$ and assume $a_n = 2^n$ for all integers $n$ such that $2 \le n \le k$.
	$a_{k+1} = 5a_{k} - 6a_{k-1}$ 
	Using the inductive hypothesis, $a_{k+1} = 5 * 2^k - 6*2^{k-1}$ = $2^{k-1}(5*2 -6)$. $2^{k-1} * 2^2 = 2^{k+1}$.

Well-ordering Principle $\equiv$ Weak Induction. WOP $\iff$ Weak Induction.
Let $S \subseteq \mathbb{N}$ be a nonempty set with $n$ elements. We do weak induction on $n$.
Base Case: 
	When $n = 1$, $S = \{a\}$ for some $a \in \mathbb{N}$, then $a$ is the smallest element of $S$. So, every subset of $\mathbb{N}$ with 1 element has a smallest element.
Induction Step:
	Let $k \ge 1$ and assume every $S \subseteq \mathbb{N}$ with $k$ elements has a smallest element. Let $S$ have $k+1$ elements. Then $S = \{a_1,a_2,...,a_{k+1}\}$. Since $S \setminus {a_{k+1}} = \{a_k\}$.