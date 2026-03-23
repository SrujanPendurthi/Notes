Let $A \in \mathbb{R}^{2\times 2}$. The determinant of $A$ is a scalar that describes the scaling and orientation of the linear transformation with matrix $A$
	The absolute value of the determinant is the scaling factor for area, volume, etc.
	The sign of the determinant is negative if $A$ causes a reflection

$\begin{pmatrix} a & b \\ c & d\end{pmatrix}$
$det(A) = ad-bc$ is True for any $2 \times 2$ matrix $A$, this is because when applying the transformation of $A$ to a square(identity matrix), we end up with a parallelogram whose sides are $v$ and $w$ with the area = $det(A)$

Let $A \in \mathbb{R}^{n \times n}$. The $(i,j)$-minor $M_{ij}$ of $A$ is the determinant of the matrix obtained by deleting row $i$ and columns $j$ from $A$

The $(i,j)$-cofactor $C_{ij}$ of $A$ is $(-1)^{i+j}M_{ij}$ 

The determinant of an $n \times n$ matrix $A$ can be computed using either of the following:
	$det(A) = \sum_{n=1}^n a_{in}C_{in}$  
	$det(A) = \sum_{n=1}^n  a_{nj}C_{nj}$  

If $A \in \mathbb{R}^{n \times n}$ is a upper or lower triangular, then the determinant of $A$ is the product of the elements on its main diagonal