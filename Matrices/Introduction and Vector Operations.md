# Definitions
**Real Vectors** are an ordered lists with a $n$ number of $\mathbb{R}$ numbers
**Components** are the elements of a vector
	Denoted $\vec{v} = \begin{pmatrix} v_1 & v_2 & v_3& ...& v_n \end{pmatrix}$
In order to say that a vector $\vec{v}$ is in a set of vectors, we say this: $\vec{v} \in \mathbb{R}^n$ 
	$\mathbb{R}^n$, the $n$ denotes the size of the vector and $\mathbb{R}$ denotes the type of number, this is defined in [[Basic Set Theory]] 

# Vector Operations
Vector Addition
	Can only add two vectors if they belong to the same set of vectors or have the same number of components, $n$
	$\vec{v} + \vec{w} = \begin {pmatrix}v_1 + w_1 & v_2 + w_2 & + ...+ & v_n + w_n \end{pmatrix}$
Scalar Multiplication
	$k\vec{v} = \begin{pmatrix} kv_1 & kv_2 \end{pmatrix}$ 
	Distribute $k$ to every component of the vector
 Dot Product 
	 $\vec{v} \cdot \vec{w} = \begin{pmatrix}v_1*w_1 &+v_2*w_2 &+...+& v_n*w_n \end{pmatrix}$
	 $\vec{v} \cdot \vec{w} = ||\vec{v}||*||\vec{w}||cos\theta$ 
	The $\theta$ is the angle between the two vectors
		If the $\theta$ is from $0 < \theta < \frac {\pi} {2}$, the angle between the two vectors is acute
		If the $\theta$ is from $\frac {\pi} {2} < \theta < \pi$, the angle between the two vectors is obtuse
		If the $\theta = \frac {\pi} {2}$, then the angle between the two vectors is orthogonal 
Magnitude
	$|| \vec{v} || = \sqrt{v_1^2+v_2^2+...+v_n^2}$
	the length of the vector
Unit Vector
	$\hat{v} = \frac{\vec{v}} {||\vec{v}||}$  
	Must always sums to 1
	Helps us find direction of vector