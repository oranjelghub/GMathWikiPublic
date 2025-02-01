---
mathLink: auto
Date created: 2024-12-08 15:35
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Linear_Algebra
cssclasses:
---

---

Proved by: _Not applicable_
References: _Not applicable_
Justifications: [[L-matrix of a linear map]], [[Linear maps]]   

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: L-matrix of a composition of linear maps is the product of their respective L-matrices
> Let $V,W,U$ be three finite dimensional $F$ vector spaces and $L:V\to W$ and $K:W\to U$ two linear maps. Then the $L$-matrix of $K\circ L$ is given by $$ K^{\beta_{U}}_{\beta_{W}} \cdot L^{\beta_{W}}_{\beta_{V}} = (K\circ L)_{\beta_{V}}^{\beta_{U}} $$

>[!quote] Proof: L-matrix of a composition of linear maps is the product of their respective L-matrices
>Let $L:V\to W$ and $K:W\to U$ be two linear maps and let $\beta_{V}$, $\beta_{W}$ and $\beta_{U}$ be bases for the three vectors spaces. We know that $K\circ L$ is also linear and thus has, per construction, a unique $L$-matrix $(K\circ L)_{\beta_{V}}^{\beta_{U}}$.We now notice that since $$ \text{co}_{\beta_{W}} \circ L = L^{\beta_{W}}_{\beta_{V}} \cdot \text{co}_{\beta_{V}} $$and $$ \text{co}_{\beta_{U}} \circ K = K^{\beta_{U}}_{\beta_{W}} \cdot \text{co}_{\beta_{W}}  $$The last equation implies that for all $w\in F^{\dim W}$ $$   (\text{co}_{\beta_{U}} \circ K\circ \text{co}_{\beta_{W}}^{-1} )(w)= K^{\beta_{U}}_{\beta_{W}} \cdot w  $$Filling this in in the first equation gives us that $$ \text{co}_{\beta_{U}}\circ K\circ L=K^{\beta_{U}}_{\beta_{W}} \cdot L^{\beta_{W}}_{\beta_{V}} \cdot \text{co}_{\beta_{V}} $$But since the $L$-matrix of a linear map is unique we know that $$ K^{\beta_{U}}_{\beta_{W}} \cdot L^{\beta_{W}}_{\beta_{V}} = (K\circ L)_{\beta_{V}}^{\beta_{U}} $$
>
>**Q.E.D.**


$$ L(v_{1})=\sum^{n}_{i=1}a_{i 1}L(v_{i}) $$