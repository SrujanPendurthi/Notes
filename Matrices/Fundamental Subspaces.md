Let $A \in \mathbb{R}^{m \times n}$. 
The <b>column space</b> of $A$ is the span of the columns of $A$, which is a subspace of $\mathbb{R}^m$. 
	The column space of $A$ is denoted $C(A)$. 
The <b>row space</b> of $A$ is the span of the rows of $A$, which is a subspace of $\mathbb{R}^n$. This is the same as the column space of $A^T$. 
	The row space of $A$ is denoted $R(A)$ 

<u>Algorithm 12.2: Bases for the Column Space and Row Space</u>
Let $A \in \mathbb{R}^{m \times n}$. 
To find a basis for the column space of $A$, put $A$ in row echelon form and then take the columns of $A$ corresponding to the pivot columns
To find a basis for the row space of $A$, put $A$ in row echelon form and then take the rows of $A$ corresponding to the rows that have pivots

<u>Theorem 12.3</u>
Let $A \in \mathbb{R}^{m \times n}$. The column space of $A$ is the set of vectors $b \in \mathbb{R}^m$ such that $Ax = b$ has at least one solution

Let $A \in \mathbb{R}^{m \times n}$. 
The <b>null space</b> of $A$ is the set of vectors $x \in \mathbb{R}^n$ with $Ax = 0$, which is a subspace of $\mathbb{R}^n$. 
	The null space of $A$ is denoted $N(A)$. 
The <b> left null space</b> of $A$ is the set of vectors $x \in \mathbb{R}^m$ with $x^TA = 0$, which is a subspace of $\mathbb{R}^m$. 
	This is the same as the null space of $A^T$
	The left null space of $A$ is denoted $N(A)^T$
<u>Algorithm 12.5: Bases for the Null Space and Left Null Space</u>
Let $A \in \mathbb{R}^{m \times n}$. 
To find a basis for the null space of $A$, find the general solution to $Ax = 0$ and then take the solution vectors being multiplied by the free variables. 
To find a basis for the left null space of $A$, do the same thing with $A^Tx = 0$ 


# Resources
[[Properties, Transpose, Inverse]]
[[Linear Independence and Bases]]
[[Vector Spaces]]
