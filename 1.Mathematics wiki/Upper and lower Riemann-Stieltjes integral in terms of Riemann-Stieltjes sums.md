---
mathLink: auto
Date created: 2024-08-07 00:50
tags:
  - Type/Object
  - Topic/Real_Analysis
cssclasses:
---

---  

Types: _Not applicable_
Examples: _Not applicable_
Construction: [[Riemann-Stieltjes integral]]
Generalization: [[Riemann-Stieltjes integral]], [[Lebesgue integral]]

Properties: _Not applicable_
Sufficiencies: _Not applicable_
Equivalences: [[Equivalence of the piecewise definition and the Riemann-Stieltjes sum definition of the upper and lower Riemann-Stieltjes integral]]
Justifications: [[Alpha-length of intervals]]

---

> [!quote] Definition: Upper and lower Riemann-Stieltjes integral in terms of Riemann-Stieltjes sums
> Let $X$ be a closed interval and let $\alpha:X\to \mathbb{R}$ be a $\alpha$-length on $X$. Let $f:I\to \mathbb{R}$ be a bounded function and let $P$ be a partition of $I$. Consider the upper and lower Riemann-stieltjes sums $$ \begin{align}  U(f,P):= \sum^{}_{J\in P}\left( \sup_{x\in J} f(x) \right) \alpha[J] \\ L(f,P):=\sum^{}_{J\in P }\left( \inf_{x\in J} f(x) \right) \alpha[J] \end{align} $$We define the upper and lower Riemann-Stieltjes integral as $$ \begin{align} \overline {\int}_{I} f\;d\alpha:=\inf\left\{ U(f,P): P\text{ is a partition of }I \right\}\\ \underline {\int}_{I} f \;d\alpha:=\sup\left\{ L(f,P):P\text{ is a partition of }I \right\}   \end{align}  $$



