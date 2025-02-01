---
mathLink: auto
Date created: 2024-10-19 21:34
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Linear_Algebra
cssclasses:
---

---

Proved by: [[Laplace or cofactor expansion]], [[Permutations change sign after composition with a transposition]]
References: _Not applicable_
Justifications: [[Determinant of a matrix (explicit permutative definition)]], [[Sign of a permutation of N]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Explicit definition of the determinant satisfies the properties of the implicit definition
> Let $\det: M_{n\times n}(F)\to F$ be the determinant map, then $\det$ satifsfies: 
> 1. $\det(\mathbb{I}_{n})=1$
> 2. $\det(C_{ij}A)=-\det (A)$
> 3. $\det$ is multilinear over the rows of $A$

 >[!quote] Proof: Explicit definition of the determinant satisfies the properties of the implicit definition
 >We start with property 1. Notice that for every permutation $\sigma\in S_{n}$, the product of elements $\prod_{1\leq i\leq n}(\mathbb{I}_{n})_{i\sigma(i)}$ is always equal to zero, unless the permutation is exactly the identity permutation $\text{Id}_{X}$. Thus $$ \det(\mathbb{I}_{n})=\text{sgn}(\text{Id}_{X})\prod_{1\leq i\leq n}(\mathbb{ I}_{n})_{ii}=1 $$ We proceed with property $2$. Let $\tau_{ij}: \mathbb{N}^{*}_{\leq n}\to \mathbb{N}^{*}_{\leq n}$ be the transposition transposing $i$ with $j$. Then we define $\sigma':=\tau_{ij}\circ \sigma$ for every $\sigma\in S_{n}$, this means $\tau_{ij}^{-1}\circ \sigma'= \tau_{ij}\circ \sigma'=\sigma$. Now we have $$ \det(C_{ij}A) =\sum^{}_{\sigma\in S_{n}}\text{sgn}(\sigma)\prod_{1\leq k\leq n}a_{\tau_{ij}(k)\sigma(k)}$$ By substituting we get $$\sum^{}_{\sigma\in S_{n}}\text{sgn}(\sigma)\prod_{1\leq k\leq n}a_{\tau_{ij}(k)\sigma(k)}= \sum^{}_{\sigma'\in S_{n}}\text{sgn}(\tau_{ij}\circ \sigma')\prod_{1\leq k\leq n}a_{\tau_{ij}(k)\tau_{ij}\circ \sigma'(k)}  $$ Notice now that the product  $\prod_{1\leq k\leq n}a_{\tau_{ij}(k)\tau_{ij}\circ \sigma'(k)}$ is exactly equal to $\prod_{1 \leq k  \ \leq n}a_{k\sigma'(k)}$. We also have that $\text{sgn}(\tau_{ij}\circ \sigma')=- \text{sgn}(\sigma')$, thus $$\sum^{}_{\sigma'\in S_{n}}\text{sgn}(\tau_{ij}\circ \sigma')\prod_{1\leq k\leq n}a_{\tau_{ij}(k)\tau_{ij}\circ \sigma'(k)}= -\sum^{}_{\sigma'\in S_{n}} \text{sgn}(\sigma')\prod_{1 \leq k  \ \leq n}a_{k\sigma'(k)}=-\det(A) $$ The third property is a almost direct consequence of the Laplace expansion. 
 >
 >**Q.E.D.**
 
 