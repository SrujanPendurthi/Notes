# LU Factorization
A is a $m*n$ matrix where no row swaps are required to put it in row echelon form then $A = LU$ where
	$L$ is a $n*n$ lower triangular matrix with 1's on the main diagonal(comes from product of elementary matrices)
	$U$ is a $m*n$ upper triangular matrix that is a row echelon form of $A
Note:
	only row operation allowed is adding a multiple of one row to a lower row(no swap, no multiples)
	Remember the shortcut for computing L(I think this is just overlaying everything)
## LU factorization with partial pivoting
$A$ is a $n *n$ matrix. We have $PA = LU$ where:
	$P$ is an $n *n$ permutation matrix
	$L$ is an $n*n$ lower triangular matrix with 1's on the diagonal
	$U$ is an $m*n$ upper triangular matrix
Using permutation matrix to swap rows because $A$ needs to be pre-swapped before $LU$ factorization
# Inverse of an elementary matrix
Let $E_{ij}(a)$ be the matrix that does $R_i+aR_j$. Then $E_{ij}(a)^{-1} = E_{ij}(-a)$

$A\vec{x} = \vec{b}$
$LU\vec{x} = \vec{b}$
$U\vec{x} = \vec{y}$
$L\vec{y}=\vec{b}$

Process:
Get $A = LU$
Solve $L\vec{y} = \vec{b}$ for $\vec{y}$
Solve $U\vec{x} = \vec{y}$ for $\vec{x}$

# Resources
[[Special Matrices]] is notes on how permutation matrices work for partial pivotingand the elementary matrices work
