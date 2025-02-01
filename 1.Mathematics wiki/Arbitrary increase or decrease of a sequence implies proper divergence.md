---
mathLink: auto
Date created: 2024-04-28 12:42
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Limsup and liminf of sequences (Properties)]]
References: _Not applicable_
Justifications: [[Limsup and liminf of sequences]], [[Proper divergent sequences]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Arbitrary increase or decrease of a sequence implies proper divergence
> Given some sequence of real numbers $(a_n)^\infty_{n=m}$
> $$ \forall M\in \mathbb{R}\;\exists N\geq m: \forall n\geq N, a_{n}\geq M \iff \liminf_{ n \to \infty }a_{n}=+\infty =\limsup_{ n \to \infty }a_{n}   $$ And for $-\infty$ $$ \forall M\in \mathbb{R}\;\exists N\geq m: \forall n\geq N, a_{n}\leq M \iff \liminf_{ n \to \infty }a_{n}=-\infty =\limsup_{ n \to \infty }a_{n}    $$

>[!quote] Proof: Arbitrary increase or decrease of a sequence implies proper divergence
>($\Leftarrow$) follows from properties of limsups and liminfs where $\forall M\in \mathbb{R}: M<\limsup_{ n \to \infty }a_{n}, \exists N\geq m: a_{n}\geq M$ for example. ($\Rightarrow$) on the other hand follows from a simple contradiction by supposing that the limsup and liming is finite (This would imply the previously mentioned property is wrong).
>
**Q.E.D.**

