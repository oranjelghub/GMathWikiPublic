---
mathLink: auto
Date created: 2025-01-17 21:10
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Linear_Algebra
cssclasses:
---
---  

Proved by: [[Laplace or cofactor expansion]]
References: _Not applicable_
Justifications: [[Eigenvalues and eigenvectors of a linear transformation]], [[Spectrum of a linear transformation]], [[Eigenspace of an eigenvalue]], [[Algebraic and geometric multiplicity of a eigenvalue]], [[Characteristic polynomial of a linear transformation]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Algebraic multiplicity of a eigenvalue is always greater than it's geometric one
> Let $V$ be a $n$-dimensional $\mathbb{C}$-vector space and $L:V\to V$ a linear transformation. If $\lambda\in \text{Spec(L)}$ then $$ 1\leq d(\lambda)\leq m(\lambda) $$Where $d(\lambda)$ denotes the geometric multiplicity and $m(\lambda)$ is algebraic multiplicity of $\lambda$.

>[!quote] Proof: Algebraic multiplicity of a eigenvalue is always greater than it's geometric one
>It is obvious that both $1\leq d(\lambda)$ and $1\leq m(\lambda)$. Now take some basis $\beta$ for $E_{\lambda}$ and expand it to a basis $\beta_{V}$ for V. With respect to $\beta_{V}$ the $L$-matrix of $L$ is obviously given by $$ L^{\beta}_{\beta}= \begin{bmatrix} \lambda \mathbb{I}_{d(\lambda)} & * \\ 0 & *\end{bmatrix} $$Which is a block matrix. If we now compute $\varphi_{L}(x)$ by expanding in the first $d(\lambda)$ columns we get that $$ \varphi_{L}(x)=(x-\lambda)^{d(\lambda)}P(x) $$It follows that $m(\lambda)$ is at least $d(\lambda)$, in other words $m(\lambda)\geq d(\lambda)$. 
>
>**Q.E.D.**