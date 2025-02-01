---
mathLink: auto
Date created: 2025-01-31 18:40
tags:
  - Type/Theorem
  - Topic/Linear_Algebra
cssclasses:
---
---  

Proved by: [[Vieta's formulas]]
References: _Not applicable_
Justifications: [[Determinant of a linear transformation]], [[Eigenvalues and eigenvectors of a linear transformation]], [[Algebraic and geometric multiplicity of a eigenvalue]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Determinant of a linear transformation is equal to the weighted product of its eigenvalues
> Let $V$ be a $n$-dimensional $\mathbb{C}$-vector space and $L:V\to V$ a linear transformation. Then $$ \det(L)=\prod_{\lambda\in \text{Spec}(L)}\lambda^{m(\lambda) }$$Where $m(\lambda)$ is the algebraic multiplicity of each eigenvalue.

Alternatively this also holds for $\mathbb{R}$-vector spaces, as long as $\varphi_{L}$ is fully factorisable. The proof is not very complicated when making use of Vieta's formulas and considering expressions for $\varphi_{L}(0)$.