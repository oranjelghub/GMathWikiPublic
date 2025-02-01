---
mathLink: auto
Date created: 2025-01-08 19:08
tags:
  - Type/Object
  - Topic/Linear_Algebra
cssclasses:
---
---  

Types: _Not applicable_
Examples: _Not applicable_
Construction: [[Characteristic polynomial of a linear transformation]]
Generalization: _Not applicable_

Properties: _Not applicable_
Sufficiencies: _Not applicable_
Equivalences: [[Eigenvalues and eigenvectors of a matrix]]
Justifications: [[Characteristic polynomial, determinant and trace of a linear transformation is independent of choice of basis]]

---

> [!quote] Definition: Eigenvalues and eigenvectors of a linear transformation
> Let $V$ be some $\mathbb{C}$-vector space and let $L: V \to V$ be a linear transfomation, we say $v \in V\backslash\{ 0 \}$ is a eigenvector with eigenvalue $\lambda \in \mathbb{C}$ if and only if 
> $$ L(v)=\lambda v $$

If we fix a basis $\alpha$ of $V$ then notice that $$ L(v)= \lambda v \iff \text{co}_{\alpha}(L (v))=\lambda \text{co}_{\alpha}(v) \iff L^{\alpha}_{\alpha}\cdot \text{co}_{\alpha}(v) =\lambda \text{co}_{\alpha}(v)$$In other words the eigenvalues of $L$ are exactly the eigenvalues of it's associated L-matrix. One may argue that this means that eigenvalues are dependent on choice of basis, but that is as it turns out not the case.

