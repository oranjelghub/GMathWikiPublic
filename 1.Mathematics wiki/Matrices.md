---
mathLink: auto
Date created: 2024-08-30 21:04
tags:
  - Type/Object
  - Topic/Linear_Algebra
cssclasses:
---

---  

Types: [[Row and reduced row echelon matrix]]
Examples: _Not applicable_
Construction: [[Determinant of a matrix (implicit definition)]], [[Determinant of a matrix (explicit permutative definition)]], [[Diagonal of a a matrix]], [[Matrix transposition]], [[Elementary matrices]], [[Matrix multiplication]], [[Trace of a matrix]], [[Left and right inverse of a matrix]]
Generalization: _Not applicable_

Properties: [[Row equivalence]]
Sufficiencies: _Not applicable_
Equivalences: _Not applicable_
Justifications: [[Existence of matrices]]

---

> [!quote] Definition: Matrix in $F$
> A matrix over a [[Fields|field]] $F$ is a rectangular array of elements of $F$.
> $$A=\begin{bmatrix} f_{11}&\ldots &f_{1n} \\ \vdots&\ddots&\vdots \\f_{m1}&\ldots& f_{mn}  \end{bmatrix}\hspace{1cm}f_{ij}\in F$$

We say this matrix has dimensions $m\times n$ ($m$ rows and $n$ columns) and refer to the elements of the matrix by specifying their position by their index: $(A)_{ij}=a_{ij}$ and the entire row by: $R_{i}$. The set, when endowed with it's standard algebra, of all $m\times n$ matrices is denoted $M_{m\times n}(F)$.

We also define matrix equality:

>[!quote] Definition: Matrix equality
>Two matrices $A$ and $B$ with dimension $m\times n$ are said to be equal if and only if: $$A=B\iff \forall i,j:1\leq i\leq m, 1\leq j\leq n,\; a_{ij}=b_{ij}$$
>We leave equality between two matrices with different dimensions undefined.



