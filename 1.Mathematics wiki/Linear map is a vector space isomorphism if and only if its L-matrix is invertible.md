---
mathLink: auto
Date created: 2024-12-08 15:04
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Linear_Algebra
cssclasses:
---
  
---

Proved by: [[L-matrix of a composition of linear maps is the product of their respective L-matrices]]
References: _Not applicable_
Justifications: [[L-matrix of a linear map]], [[Vector space isomorphism]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Linear map is a vector space isomorphism if and only if its L-matrix is invertible
> Let $V,W$ be two finite dimensional $F$-vector spaces of such that $V\cong W$. Then some linear map $L:V\to W$ is a vector space isomorphism if and only if the $L$-matrix of $L$ is invertible. Furthermore if $L$ is a isomorphism and $\beta_{V}$ and $\beta_{W}$ are bases of $V$ and $W$, then $$ (L^{-1})_{\beta_{W}}^{\beta_{V}}=(L^{\beta_{W}}_{\beta_{V}})^{-1} $$

>[!quote] Proof: Linear map is a vector space isomorphism if and only if its L-matrix is invertible
>Suppose first that $L$ is a isomorphism, then it has some inverse $L^{-1}$ which has a $L$-matrix $(L^{-1})^{\beta_{V}}_{\beta_{W}}$. We then have $$ L^{\beta_{W}}_{\beta_{V}}\cdot (L^{-1})^{\beta_{V}}_{\beta_{W}}=(L\circ L^{-1})^{\beta_{W}}_{\beta_{W}}=(\text{Id}_{W})^{\beta_{W}}_{\beta_{W}}=\mathbb{I}_{\dim V}=\mathbb I_{\dim W} $$Thus if $V\cong W$ then clearly $(L^{-1})_{\beta_{W}}^{\beta_{V}}=(L^{\beta_{W}}_{\beta_{V}})^{-1}$. It remains to show that $L$ is a isomorphism if it's $L$-matrix is invertible. If $L^{\beta_{W}}_{\beta_{V}}$ is invertible then we know that it's inverse can uniquely be associated with some linear map $K:W\to V$. It is not hard to see that $$ K\circ L = \text{Id}_{W} $$and $$ L\circ K= \text{Id}_{V} $$Thus $L$ is invertible, meaning it is bijective and thus a vector space isomorphism.
>
>**Q.E.D.**