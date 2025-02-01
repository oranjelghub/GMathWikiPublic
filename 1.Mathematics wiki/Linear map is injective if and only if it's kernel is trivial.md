---
mathLink: Linear map is injective if and only if $\text{ker}(L)=\{0\}$
Date created: 2024-12-08 17:17
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Linear_Algebra
cssclasses:
---

---

Proved by: _Not applicable_
References: _Not applicable_
Justifications: [[Kernel of a linear map]], [[Linear maps]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Linear map is injective if and only if $\text{ker}(L)=\{0\}$
> Let $V,W$ be $F$-vector spaces and $L:V\to W$ a linear map. Then $L$ is injective if and only if $$ \text{ker}(L)=\{ 0 \} $$

>[!quote] Proof: Linear map is injective if and only if $\text{ker}(L)=\{0\}$
>Suppose first that $L$ is injective. We already know that $\{ 0 \}\subset \text{ker}(L)$. Let $\alpha\in \text{ker}(L)$ then $$ L(\alpha)=0=L(0) $$Implying $\alpha=0$ by the injectivity of $L$. Thus $\text{ker}(L)=\{ 0 \}$. Suppose on the other hand that $\text{ker}(L)=\{ 0 \}$. Given any two vectors $v,w\in V$ such that $L(v)=L(w)$ we have $$ L(v-w)=0 \implies v-w\in \text{ker(L)}$$Thus $v=w$, implying $L$ is injective.
>
>**Q.E.D.**

 