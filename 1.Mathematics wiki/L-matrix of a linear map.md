---
mathLink: auto
Date created: 2024-11-18 12:51
tags:
  - Type/Object
  - Topic/Linear_Algebra
cssclasses:
---

---  

Types: _Not applicable_
Examples: _Not applicable_
Construction: _Not applicable_
Generalization: _Not applicable_

Properties: [[L-matrix of a composition of linear maps is the product of their respective L-matrices]], [[Linear map is a vector space isomorphism if and only if its L-matrix is invertible]]
Sufficiencies: _Not applicable_
Equivalences: _Not applicable_
Justifications: [[Linear maps are uniquely determined by a matrix once two bases are fixed]]

---

> [!quote] Definition: L-matrix of a linear map
> Let $V,W$ be some finite dimensional $F$-vector spaces with bases $\beta_{V}$ and $\beta_{W}$ respectively and $L:V\to W$ a linear map, then the associated $L$-matrix is the unique $A\in M_{\dim W\times \dim V}(F)$ such that $$ \text{co}_{\beta_{W}}\circ L=  A\circ \text{co}_{\beta_{V}} $$
> We often write this matrix $L^{\beta_{W}}_{\beta_{V}}$. This matrix is built out of columns which are specifically the column vectors $\text{co}_{\beta_{W}}(L(v_{i}))$ where $v_{i}$ is a basis vector in $\beta_{V}$.

