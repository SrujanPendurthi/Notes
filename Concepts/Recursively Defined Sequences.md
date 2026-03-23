Let $A$ be a set. Let $f: \mathbb{N} \to A$ be function. The list $f(0), f(1), f(2),...$ is called a sequence in $A$. We usually denote $f(i)$ by $a_i$

A recursively-defined sequence is a sequence whose $n^{th}$ term is defined using previous terms

The Fibonacci sequence is defined as follows:
	$f_1, f_2 = 1, f_n = f_{n-1} + f_{n-2}$$

Let $n \in \mathbb{N}$. The factorial of $n$ is defined recursively by: $0! = 1$ and $n! = n *(n-1)!$

Let $n,m \in \mathbb{Z}$ with $n \ge m$. Let $a_m,a_{m+1},...,a_n \in \mathbb{R}$. Define $\sum_{i=m}^n a_i$ and $\prod_{i = m}^n a_i$ recursively by: 
	$\sum_{i=m}^m a_i = a_m$ and $\sum_{i=m}^n a_i = a_n + \sum_{i=m}^{n-1} a_i$ 
	$\prod_{i = m}^m a_i = a_m$ and $\prod_{i = m}^n a_i = a_n * \prod_{i = m}^{n-1} a_i$ 

Well Ordering Principle: Every nonempty subset of $\mathbb{N}$ has a smallest element