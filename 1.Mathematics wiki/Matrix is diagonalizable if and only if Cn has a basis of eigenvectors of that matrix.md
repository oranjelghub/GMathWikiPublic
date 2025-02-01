---
mathLink: Matrix is diagonalizable if and only if $\mathbb C^n$ has a basis of eigenvectors of that matrix
Date created: 2025-01-17 18:11
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Linear_Algebra
cssclasses:
---
---  

Proved by: [[L-matrix of a linear map]]
References: _Not applicable_
Justifications: [[Eigenvalues and eigenvectors of a matrix]], [[Diagonalizable matrices]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Matrix is diagonalizable if and only if $\mathbb C^n$ has a basis of eigenvectors of that matrix
> Let $A \in M_{n\times n}(\mathbb{\mathbb{C}})$, then $A$ is diagonalizable if and only if $\mathbb{\mathbb{C}}^{n}$ has a basis of eigenvectors of $A$.

>[!quote] Proof: Matrix is diagonalizable if and only if $\mathbb C^n$ has a basis of eigenvectors of that matrix
>Suppose first that $A$ is diagonalizable. Then we have that $$ A \cdot P=P\cdot D $$for some diagonal matrix $D$. It follow that every column of $P$, namely $p_{i}$, satisfies $$ Ap_{i}=\lambda_{i}p_{i} $$Where $\lambda_{i}$ is the entry in the $i$'th column of $D$. Thus we see that every column $p_{i}$ is a eigenvector (since it has to be non-zero) with eigenvalue $\lambda_{i}$. It suffices to now that $\{ p_{i} \}_{1\leq i\leq n}$ is a basis for $\mathbb{C}^n$. This is not hard, because the fact that $P$ is invertible implies that it's columns are free, thus forming a basis since we have $n$ of them. Now suppose on the other hand that $\mathbb{C}^{n}$ has a basis $\beta$ of eigenvectors of $A$. Denote $\alpha$ the standard basis of $\mathbb{C}^{n}$, then $(L_{A})^{\alpha}_{\alpha}=A$ on the other hand $(L_{A})^{\beta}_{\beta}=D$ is some diagonal matrix. But we know that those matrices must be similar by using the matrix of change of basis $$ (\text{Id})_{\beta}^{\beta}\cdot (L_{A})^{\alpha}_{\alpha} \cdot(\text{Id})_{\beta}^{\alpha}=(L_{A})^{\beta}_{\beta} $$Thus $A$ is similar to some diagonal matrix $D$ and is thus diagonalizable. 
>
>**Q.E.D.**
