---
mathLink: auto
Date created: 2025-01-17 21:26
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Linear_Algebra
cssclasses:
---
---  

Proved by: [[Fundamental theorem of algebra]], [[Algebraic multiplicity of a eigenvalue is always greater than it's geometric one]], [[Eigenvectors with different eigenvalues are free]]
References: _Not applicable_
Justifications: [[Spectrum of a linear transformation]], [[Diagonalizable linear transformations]], [[Eigenspace of an eigenvalue]], [[Algebraic and geometric multiplicity of a eigenvalue]]  

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Linear transformation is diagonalizable if and only if the algebraic and geometric multiplicity of each eigenvalue are equal
> Let $V$ be a $n$-dimensional $\mathbb{C}$-vector space and $L:V\to V$ a linear transformation. Then $L$ is diagonalizable if and only if $$ \forall \lambda \in \text{Spec}(L): d(\lambda)=m(\lambda) $$

>[!quote] Proof: Linear transformation is diagonalizable if and only if the algebraic and geometric multiplicity of each eigenvalue are equal
>We first assume that $L$ is diagonalizable and prove that $$ \forall \lambda \in \text{Spec}(L): d(\lambda)=m(\lambda) $$Take some basis of eigenvectors $\beta$ of $L$ for $V$. Then $$ L^{\beta}_{\beta}=\begin{bmatrix} \lambda_{1}& \dots& 0  \\ \vdots & \ddots &\vdots   \\ \\ 0 & \dots & \lambda_{n}\end{bmatrix} $$Now index for each $\lambda_{i}\in \text{Spec}(L)$ all the eigenvalues $\{ \lambda_{i_{j}} \}_{1\leq j \leq k_{i}}$ of the basis vectors of $\beta$ which have eigenvalue $\lambda_{i}$. Then we have$$ \varphi_{L}(x)=\prod_{1\leq i\leq l}\prod_{1\leq j\leq k_{i}}(x-\lambda_{i_{j}}) =\prod_{1\leq i\leq l}(x-\lambda_{i})^{k_{i}}$$We thus see that $m(\lambda_{i})=k_{i}$, but at the same time $k_{i}$ is also the amount of eigenvectors in $\beta$ which have eigenvalue $\lambda_{i}$. Since those vectors are all free, we conclude that $d(\lambda_{i})=k_{i}=m(\lambda_{i})$. Now assume on the other hand that $$  \forall \lambda \in \text{Spec}(L): d(\lambda)=m(\lambda)  $$We know that $$ \varphi_{L}(x)=\prod_{1\leq i\leq k} (x-\lambda_{i})^{m(\lambda_{i})}$$with $d(\lambda_{i})=m(\lambda_{i})$ by assumption. Now for each eigenvalue $\lambda_{i}$ take some basis $\{ v_{i,j} \}_{1\leq j \leq m(\lambda_{i}) }$ of the eigenspace $E_{\lambda_{i}}$. We now claim that $\bigcup_{1\leq i\leq k}\{ v_{i,j} \}_{1\leq j \leq m(\lambda_{i}) }$ forms a basis for $V$. We notice that this set consists of exactly $\sum^{k}_{i=1}m(\lambda_{i})$ elements which, because we are in $\mathbb{C}$, is exactly equal to $\dim V= n$. It thus suffices to show that $\bigcup_{1\leq i\leq k}\{ v_{i,j} \}_{1\leq j \leq m(\lambda_{i}) }$ is free, so assume that $$ \sum^{k}_{i=1}\sum^{m(\lambda_{i})}_{j=1} \mu_{i,j} v_{i,j}=0$$We can write this as $$ \sum^{k}_{i=1}u_{i}=0 $$Where each $u_{i}$ is a vector in $E_{\lambda_{i}}$. But since all those eigenvectors have distinct eigenvalues we must have that each $u_{i}=0$. But since each set of $\{ v_{i,j} \}_{1\leq j \leq m(\lambda_{i})}$ also forms a basis for $E_{\lambda_{i}}$ we also have that each $\mu_{i,j}=0$, proving that $\bigcup_{1\leq i\leq k}\{ v_{i,j} \}_{1\leq j \leq m(\lambda_{i})}$ is free.
>
>**Q.E.D.**

