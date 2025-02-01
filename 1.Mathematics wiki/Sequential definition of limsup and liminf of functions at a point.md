---
mathLink: auto
Date created: 2024-05-17 16:49
tags:
  - Type/Object
  - Topic/Real_Analysis
cssclasses:
---

---  

Types: _Not applicable_
Examples: _Not applicable_
Construction: _Not applicable_
Generalization: _Not applicable_

Properties: _Not applicable_
Sufficiencies: _Not applicable_
Equivalences: [[Limit of a real valued function at a point]]
Justifications: [[Limsup and liminf of functions at a point]], [[Limit of a sequence]], [[Equivalence between the sequential and the classic definition of the limsup and liminf of a function at a point]]

---

> [!quote] Definition: Sequential definition of limsup and liminf of functions at a point
> Given $E\subseteq X\subseteq \mathbb R$, $x_0\in \overline E$, and a function $f:X\to \mathbb R$. We say $\limsup_{x\to x_0:x\in E}f(x)=L$ if and only if there exists a sequence $(x_n)_{n=m}^\infty$ consisting of only elements in $E$ that also converges to $x_0$, such that $\lim_{n\to \infty}f(x_n)=L$ and such that for all other sequences $(y_n)_{n=m}^\infty$ that consist of elements of $E$, converge to $x_0$ and induce a convergent sequence $(f(y_n))_{n=m}^\infty$, we have $$\lim_{n\to \infty}f(y_n)\leq \lim_{n\to \infty}f(x_n)=L$$

The sequential limit inferior is defined similarly.

