---
mathLink: auto
Date created: 2024-11-05 21:22
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Linear_Algebra
cssclasses:
---

---

Proved by: _Not applicable_
References: _Not applicable_
Justifications: [[Matrix multiplication]], [[Bases of vector spaces]], [[Dimension of a vector space]], [[Linear maps]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Linear transformations are uniquely determined by a a matrix once a two bases are fixed
> Let $L:V\to W$ be a linear map from two finite-dimensional $F$-vector spaces with a fixed basis $\beta_{V}$ for $V$ and a fixed basis $\beta_{W}$ for $W$. Then there exists some unique matrix $L^{\beta_{W}}_{\beta_{V}}$ such that $$\text{co}_{\beta_{W}}\circ L=  L^{\beta_{W}}_{\beta_{V}} \circ \text{co}_{\beta_{V}}$$

>[!quote] Proof: Linear transformations are uniquely determined by a a matrix once a two bases are fixed
>Per convention, when talking about coordinate vectors they will always be in column form. We write $n=\dim V$ and $m=\dim W$. We can then say that $$ v=\sum^{n}_{i=1}x_{i}v_{i}\hspace{2 cm} L(v)=\sum^{m}_{i=1}y_{i}w_{i} $$This can we written as $$ v=(v_{i})_{1\leq i\leq n}\cdot \begin{bmatrix}x_{1} \\ \vdots \\ x_{n} \end{bmatrix}  \hspace{2 cm } L(v)= (w_{i})_{1\leq i\leq m}\cdot \begin{bmatrix} y_{1}\\ \vdots \\ y_{m} \end{bmatrix}$$ By the linearity of $L$ we also have $$ L(v)=\sum^{n}_{i=1}x_{i}L(v_{i})= (L(v_{i}))_{1\leq i\leq n}\cdot\begin{bmatrix} x_{1} \\ \vdots \\ x_{n} \end{bmatrix} $$ But at the same time each $L(v_{i})$ is just some vector in $W$ and thus we can write it as $$ L(v_{i})=(w_{i})_{1\leq i\leq m}\cdot \begin{bmatrix} a_{1i} \\ \vdots \\ a_{mi} \end{bmatrix} $$Thus we may write $$ (L(v_{i}))_{1\leq i\leq n}=(w_{i})_{1\leq i\leq m} \cdot \begin{bmatrix} a_{11} &  \dots &  a_{1n} \\ \vdots & \ddots & \vdots\\ a_{m 1} & \dots & a_{mn} \end{bmatrix}$$We call this matrix $L^{\beta_{W}}_{\beta_{V}}$, clearly it is uniquely determined. We can now fill in this definition to obtain $$\begin{bmatrix} y_{1}\\ \vdots \\ y_{m} \end{bmatrix}=L^{\beta_{W}}_{\beta_{V}}\cdot \begin{bmatrix}x_{1} \\ \vdots \\ x_{n} \end{bmatrix}  $$ One could now manually verify that indeed $$ \text{co}_{\beta_{W}}\circ L=  L^{\beta_{W}}_{\beta_{V}} \circ \text{co}_{\beta_{V}} $$
>
>**Q.E.D.**



