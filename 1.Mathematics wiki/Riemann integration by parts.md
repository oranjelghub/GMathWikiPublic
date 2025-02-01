---
mathLink: auto
Date created: 2024-09-25 12:33
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Second fundamental theorem of calculus]], [[Uniformly continuous functions on bounded intervals are Riemann integrable]], [[product ru]]
References: _Not applicable_
Justifications: [[Riemann integral]], [[Differentiation of real valued functions]]

Specializations: _Not applicable_
Generalizations: [[Lebesgue integration by parts]]

---

> [!quote] Theorem: Riemann integration by parts
> Let $I=[a,b]$, and let $F:[a,b]\to \mathbb{R}$ and $G:I\to \mathbb{R}$ be differentiable functions on $[a,b]$, such that $F^{'}$ and $G^{'}$ are Riemann integrable on $I$, then we have $$ \int_{[a,b]} FG'=F(b)G(b)-F(a)G(a)-\int_{[a,b]} F^{'}G $$

>[!quote] Proof: Riemann integration by parts
>Notice first that since $F$ and $G$ are both differentiable on $[a,b]$, that they are uniformly continuous on $[a,b]$, and thus Riemann integrable on $[a,b]$. It follows that the functions $FG^{'}$ and $F^{'}G$ are both Riemann integrable. Now consider the following integral $$ \int_{[a,b]} FG^{'}+F^{'}G $$By the product rule we have $$ \int_{[a,b]} (FG)^{'} $$Clearly $FG:[a,b]\to \mathbb{R}$ is the anti derivative of $(FG)'$ and $(FG)'$ is Riemann integrable on $[a,b]$. By the second fundamental theorem of calculus it thus follows that $$  \int_{[a,b]} (FG)^{'} =F(b)G(b)-F(a)G(a) $$Or more generally $$ \int_{[a,b]} FG'=F(b)G(b)-F(a)G(a)-\int_{[a,b]} F^{'}G  $$
>
>**Q.E.D.**
