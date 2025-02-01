---
mathLink: auto
Date created: 2025-01-16 15:46
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Linear_Algebra
cssclasses:
---
---  

Proved by: [[Determinant of a matrix (Properties)]], [[Trace of a product of matrices]]
References: _Not applicable_
Justifications: [[Determinant of a linear transformation]], [[Trace of a linear transformation]], [[Characteristic polynomial of a linear transformation]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Characteristic polynomial, determinant and trace of a linear transformation is independent of choice of basis
> Let $V$ be a $F$-vector space and $L:V\to V$ a linear transformation. Then for any two choices of bases $\alpha$ and $\beta$ we have
> $$ \begin{align} \mathrm{Tr}(L^{\alpha}_{\alpha})&=\mathrm{Tr}(L^{\beta}_{\beta}) \\  \det(L^{\alpha}_{\alpha})&=\det(L^{\beta}_{\beta}) \\ \varphi_{L^{\alpha}_{\alpha}}(x) &=\varphi_{L^{\beta}_{\beta}}(x) \end{align} $$

>[!quote] Proof: Characteristic polynomial, determinant and trace of a linear transformation is independent of choice of basis
>We can use the matrix of basis change to write $$ L^{\alpha}_{\alpha}=(\text{Id}^{\beta}_{\alpha})^{-1}\cdot L^{\beta}_{\beta}\cdot\text{Id}^{\beta}_{\alpha} $$Using basic properties of the trace and the determinant we get $$ \det(L^{\alpha}_{\alpha})=\det((\text{Id}^{\beta}_{\alpha})^{-1}\cdot L^{\beta}_{\beta}\cdot\text{Id}^{\beta}_{\alpha} )=\det(L^{\beta}_{\beta}) $$ and $$ \mathrm{Tr}(L^{\alpha}_{\alpha})=\mathrm{Tr}((\text{Id}^{\beta}_{\alpha})^{-1}\cdot L^{\beta}_{\beta}\cdot\text{Id}^{\beta}_{\alpha})=\mathrm{Tr}((\text{Id}^{\beta}_{\alpha})^{-1}\cdot\text{Id}^{\beta}_{\alpha}\cdot L^{\beta}_{\beta})=\mathrm{Tr}(L^{\beta}_{\beta}) $$Furthermore we know that $$ \varphi_{L^{\alpha}_{\alpha}}(x)=\det(x\mathbb{I}-L^{\alpha}_{\alpha})=\det(x\mathbb{I}-(\text{Id}^{\beta}_{\alpha})^{-1}\cdot L^{\beta}_{\beta}\cdot\text{Id}^{\beta}_{\alpha}) $$ And since $x$ is just some vector we can write $$ \varphi_{L^{\alpha}_{\alpha}}(x)=\det((\text{Id}^{\beta}_{\alpha})^{-1}\cdot (x\mathbb{I}-L^{\beta}_{\beta})\cdot\text{Id}^{\beta}_{\alpha})=\varphi_{L^{\beta}_{\beta}}(x) $$
>This closes the proof
>
>**Q.E.D.**

