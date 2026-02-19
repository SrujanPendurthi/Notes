# Definition
A **Set** is a well-defined collection of objects, considered as a single object in its own right.
	The objects in a set are called **Elements**(or members). 
	A set is well-defined if we can ambiguously decide whether any object belongs to the set
	Notated commonly using capital letters for sets and lowercase letters to denote elements

Sets are a foundational concept in mathematics.

In formal set theory, a set is treated as an undefined primitive, with its properties and behavior described by axioms

How to define a set?
"Let [Set Name Here] be a set such that [condition here]"

# Notation
**Roster Notation** lists all elements of a set explicitly, meaning that all elements must be written out
	*Example: S = {2,4,5,7,8,9}*
	Very straightforward for sets with small number of elements, but impractical for sets with large number of elements
	When sets have a clear and recognizable pattern, we may use an informal 'implied list' notation with ellipses
		*Example: S = {1,2,3,4,5,...}*
**Set-Builder Notation** provides a more flexible and precise way to define sets, especially with infinite elements
	Describes the properties that characterize the elements of the set using a predicate
	$S = \{x\in A|P(x)\}$ or $S = \{x \in A: P(x)\}$
	On the left side of the colon, we indicate which set our elements are coming from.
	On the right side of the colon, we indicate the properties the elements must hold
# Set Equality
$A=B \iff$   
	Every element of A is an element of B
	Every element of B is an element of A

Order, repetition, and set presentation are NOT pertinent for Set equality 

$A = B \iff A \subseteq B \wedge B \subseteq A$

$\subset$ is not the same as $\subseteq$ as the second symbol indicates equality, while the first one does not. The first one indicates that the sets are not equal that one is a subset of another

$\subset$ is defined as $\forall a \in A, a \in B$
$\subsetneq$ is defined as $([\forall a \in A, a \in B] \land [\exists b \in B, b \notin A])$
The $\subseteq$ relation has a property known as **transitivity**

**Transitivity Theorem:** If $A \subseteq B$ and $B \subseteq C$, then $A \subseteq C$

*Proof for Transitivity:* 
	Assume that A,B, and C are arbitrary sets with the properties that $A \subseteq B$ and $B \subseteq C$.
	We want to show that $A \subseteq C$.
	Let $a \in A$ such that $a$ is an arbitrary element, allowing us to use the reasoning on $a$ to every element in $A$. 
	Since we are given that $A \subseteq B$, we know that every element in $A$ must be an element in $B$ by definition of $\subseteq$. 
	Thus, we are given $a \in B$ such that $a$ is an arbitrary element.
	Repeating this same logic to $C$, we arrive that $A \subseteq C$, since every element of $A$ is an element of $C$ due to the fact that we chose $a$ as arbitrary.
# Number Sets
## Natural Numbers
There are several sets of numbers that are so commonly used that they get a fixed notation

$\mathbb{N}$ is the natural number set, meaning any integer from 0 to infinity.

$\mathbb{N}$ is defined to be the smallest set containing 0 and closed under the successor function(the +1 function).
	Informally, the natural numbers are the points on the number line
	Properties:
		There is no largest natural number
		0 is the smallest natural number
		The sum of two natural numbers is a natural number(closed under addition)
		The product of two natural numbers is a natural number(closed under multiplication)
## Integers
$\mathbb{Z}$ is used to denote the set of all integers, a set of all natural numbers and their additive inverses(their negatives)
	Properties:
		There is no smallest nor largest natural number
		The sum, difference, and product of any two integers is an integer

**Integer Divisibility:** For $a,b \in \mathbb{Z}$, we say that $a$ divides $b$, denoted $a|b$, if and only if there exists an integer, $c$,  such that $b = ac$.
	Using Integer Divisibility, we can define every integer as odd/even
	**Even** $\iff 2|n$ 
	**Odd** $\iff 2\nmid n$

**Transitivity of Divisibility:** For any $a, b,c \in \mathbb{Z}$, if $a|b$ and $b|c$, then $a|c$
	*Proof:*
		Assume $a,b, c \in \mathbb{Z}$ such that $a|b$ and $b|c$. Then, by definition of integer divisibility, $b = ma$ and $c = nb$ such that $m$ and $n$ $\in \mathbb{Z}$. Using algebra, we get $c = mna$, then we can get $c = da$ such that $d$ is the integer product of $m$ and $n$. Since $c = da$, $a|c$ 

**Division Algorithm:** Let $a, b, c \in \mathbb{Z}$ with $b\neq 0$. Then there exist unique integers $q$ and $r$  such that $a =bq +r$ with $0 \le r < |b|$. Here, $q$ is called the quotient and $r$ is referred to as the remainder
	This theorem formalizes the division with remainder

n many integers is denoted as $[n]$
	This means a set of integers from 1 to n inclusive

## The Rational Numbers

$$\mathbb{Q} = \{\frac {a} {b}|a,b\in \mathbb{Z}\text{ and }b \neq 0\}$$


Since $\mathbb{Q}$ have a strong connection with $\mathbb{Z}$, we can get many properties of $\mathbb{Q}$ from $\mathbb{Z}$.

**Properties:**
	The sum(or difference) of two rational numbers is a rational number
	The product of two rational numbers is a rational number
	The quotient of two rational numbers, where the divisor is a nonzero, is a rational number

## The Real Numbers
$\mathbb{R}$ denotes the set of real numbers. This set includes all of $\mathbb{Q}$, as well as all irrational numbers

## The Empty Set
$\emptyset$ denotes the empty set, which is the unique set with no elements

# Resources
https://www.youtube.com/watch?v=tyDKR4FG3Yw&list=PLDDGPdw7e6Ag1EIznZ-m-qXu4XX3A0cIz

[[Sets]]