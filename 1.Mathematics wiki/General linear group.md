
Let $GL(n,\mathbb{R})$ be the [[Sets|set]] of all $n\times n$ [[Matrices|matrices]] with real entries and a non-zero [[Determinant of a matrix (implicit definition)|determinant]]. Then we can show that under the [[Binary operations|operation]] of matrix multiplication, $GL(n,\mathbb{R})$ forms a [[Groups|non-abelian group]].



## Case of $n=2$

We here have the set:
$$GL(2,\mathbb{R})=\left\{\begin{bmatrix} a & b \\ c & d\\\end{bmatrix}:a,b,c,d\in R\land ad-bc\neq 0\right\}$$
This set forms a [[Groups|group]] as:
$$\begin{bmatrix}a_1 & b_1 \\c_1 &d_1\end{bmatrix}\begin{bmatrix}a_2 & b_2 \\c_2&d_2\end{bmatrix}=\begin{bmatrix}a_1a_2+b_1c_1&a_1b_2+b_1d_2\\c_1a_2+d_1c_2&c_1b_2+d_1d_2\end{bmatrix}$$
Which also has a non-zero [[Determinant of a matrix (implicit definition)|determinant]] since $det(A)det(B)=det(AB)$.
The Identity is $\begin{bmatrix}1&0\\0&1\end{bmatrix}$ and the inverse is:
$$\begin{bmatrix}\frac{d}{ad-bc}&\frac{-b}{ad-bc}\\\frac{-c}{ad-bc}&\frac{a}{ad-bc}\end{bmatrix}$$
Which also has a non-zero [[Determinant of a matrix (implicit definition)|determinant]] as $det(A^{-1})=det(A)^{-1}$.


