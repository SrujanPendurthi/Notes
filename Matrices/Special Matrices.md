# Triangular and Diagonal Matrices
A matrix is **upper triangular** if all entries below its main diagonal are 0
	Equivalently, $a_{ij} = 0$ when $i > j$
A matrix is **lower triangular** if all entries above its main diagonal are 0
	Equivalently, $a_{ij} = 0$ when $i < j$
A matrix is **diagonal** if all entries not on the main diagonal are 0
	Equivalently, $a_{ij} = 0$ when $i \ne j$
	Multiplying a square diagonal matrix on the left:
		Multiples the rows by the number on the diagonal
		Basically, distributing the diagonal entry across
	Multiplying a square diagonal matrix on the right:
		Multiple the columns by the number on the diagonal
		Basically, distributing the diagonal entry down

Multiplying two special matrices of the same type results in the same type of special matrix

# Permutation Matrix
A $n * n$ matrix is a **permutation matrix** if it has exactly one 1 in each row and column and all other entries are zero

Multiplying a permutation matrix on the left permutes the rows
	Basically, moves all the rows down one, pushing the bottom one to the top
Multiplying a permutation matrix on the left permutes the columns
	Basically, pushes all the columns one to the right

# Symmetric and Skew-Symmetric Matrices
A $n * n$ matrix $A$ is **symmetric** if $A^T = A$
A $n * n$ matrix $A$ is **skew-symmetric** if $A^T = -A$

# Elementary Matrices
An **elementary matrix** is a $n * n$ matrix $E$ where the product $EA$ performs an elementary row operation on matrix $A$

There are three types:
	For swapping two rows
	For multiplying a row by a nonzero constant
	For adding a constant multiple of one row to another row

*For swapping two rows*:
	To swap row $i$ and row $j$, use the permutation matrix $P_{ij}$ that looks like the identity matrix with rows $i$ and $j$ switched

*For multiplying a row by a nonzero constant*:
	To multiply row $i$ by the constant $a$, use the diagonal matrix $D_i(a)$ that looks like the identity matrix except for the entry $d_{ii} = a$

*For adding a constant multiple of one row to another row*:
	To add $a$ times row $j$ to row $i$, use the matrix $E_{ij}(a)$ that looks like the identity matrix except for the entry $e_{ij} = a$

# Resources
https://www.youtube.com/watch?v=3njO5_vyMjw

[[Elementary Row Operations and Gaussian Elimination]] this is what elementary matrices and permutation matrices do