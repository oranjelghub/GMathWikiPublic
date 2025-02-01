---
mathLink: auto
Date created: 2024-10-08 14:10
tags:
  - Type/Theorem
  - Type/Proof
cssclasses:
---

---

Proved by: [[Sign of a permutation of N]], [[Symmetric groups]]
References: _Not applicable_
Justifications: [[Determinant of a matrix (implicit definition)]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Uniqueness of the determinant map
> Let $f:M_{n \times n}(F)\to F$ be a function satisfying the properties down below, then $f$ must be the explicit determinant map, given by $$ \det(A)=\sum^{}_{\sigma\in S_{n}} \left( \text{sgn}(\sigma)\prod_{1\leq i\leq n}a_{i\sigma(i)} \right)$$Properties:
> 1. $f(\mathbb{I}_{n})=1$
> 2. $f(C_{ij}A)=-f (A)$
> 3. $f$ is multilinear over the rows of $A$

 >[!quote]- Proof: Uniqueness of the determinant map
 > Let $A$ be some matrix in $M_{n\times n}(F)$, we define for all $1\leq k\leq n$ the rows $$ e_{k}:=(b_{i})_{1\leq i\leq n} $$Where $b_{i}=0$, unless $i=k$, then $b_{k}=1$. We can then write every row of $A$ as $$ R_{j}=\sum^{n}_{i=1}a_{ji}e_{i} $$According to the multilinearity of $f$, we have that $$ f(A)= \sum^{n}_{j_{1}=1}a_{1j_{1}} f\left( \begin{bmatrix} e_{j_{1}}\\ \sum^{n}_{j_{2}=1}a_{2j_{2}}e_{j_{2}} \\ \vdots \\\sum^{n}_{j_{n}=1}a_{nj_{n}}e_{j_{n}}\end{bmatrix} \right)$$Inductively it follows that $$ f(A)=\sum^{n}_{j_{1}\dots j_{n}=1} \prod^{n}_{l=1} a_{lj_{l}}f\left(\begin{bmatrix} e_{j_{1}}\\ \vdots \\e_{j_{n}}\end{bmatrix}\right) $$Notice also that $f\left(\begin{bmatrix} e_{j_{1}}\\ \vdots \\e_{j_{n}}\end{bmatrix}\right)$ is equal to zero whenever there are equal rows. This means that the entire sum can be restricted. Specifically, each non-zero term of the sum can we written as $$ \prod^{n}_{l=1} a_{lj_{\sigma(l)}}f\left(\begin{bmatrix} e_{j_{\sigma(1)}}\\ \vdots \\e_{j_{\sigma(n)}}\end{bmatrix}\right) $$Where $\sigma$ is the permutation that assigns to every index $l$ the unique value $j_{\sigma(l)}$ for which this product is non-zero. We can thus write $$ \sum^{}_{\sigma\in S_{n}}\prod^{n}_{l=1} a_{lj_{\sigma(l)}}f\left(\begin{bmatrix} e_{j_{\sigma(1)}}\\ \vdots \\e_{j_{\sigma(n)}}\end{bmatrix}\right) $$Where $S_{n}$ is the symmetric group of order $n$. We can also write $\begin{bmatrix} e_{j_{\sigma(1)}}\\ \vdots \\e_{j_{\sigma(n)}}\end{bmatrix}$as collection of elementary row operations on $\mathbb{I}_{n}$. Namely, for every non-identity mapping of $\sigma$, we can write $$ f\left(\begin{bmatrix} e_{j_{\sigma(1)}}\\ \vdots \\e_{j_{\sigma(n)}}\end{bmatrix}\right)=f\left(\prod_{1\leq i\leq n: \sigma(i)\neq i}C_{i\sigma(i)}\mathbb{I}_{n}\right)=(-1)^{m} $$Where $m$ is the number of $C_{ij}$ matrices in the product. But notice that each of the $C_{ij}$ matrices represents an inversion of $\sigma$. Thus we have $$ f\left(\prod_{1\leq i\leq n: \sigma(i)\neq i}C_{i\sigma(i)}\mathbb{I}_{n}\right)=(-1)^{m} =(-1)^{\#\text{Inv}(\sigma)} =\text{sgn}(\sigma)$$This means that $$ f(A)=\sum^{}_{\sigma\in S_{n}}\prod_{1\leq i\leq n} a_{ij_{\sigma(i)}}f\left(\begin{bmatrix} e_{j_{\sigma(1)}}\\ \vdots \\e_{j_{\sigma(n)}}\end{bmatrix}\right)=\sum^{}_{\sigma\in S_{n}} \text{sgn}(\sigma) \prod_{1\leq i\leq n} a_{ij_{\sigma(i)}} $$This implies that every determinant map is of the same map and is thus unique.
 > 
 > **Q.E.D.**
