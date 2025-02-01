---
mathLink: auto
Date created: 2024-05-25 16:54
tags:
  - Type/Notion
  - Topic/Real_Analysis
cssclasses:
---

---

Types: _Not applicable_
Examples: _Not applicable_
Construction: _Not applicable_
Generalization: _Not applicable_

Properties: [[Real valued function is continuous at a point if and only if the left and right limit agree with the function value at that point]]
Sufficiencies: _Not applicable_
Equivalences: _Not applicable_
Justifications: [[Limit of a real valued function at a point]]

---

> [!quote] Notion: Left and right limits of real valued functions
> Let $X$ be a subset of $\mathbb{R}$, $f : X → \mathbb{R}$ be a function, and let $x_{0}$ be a real number. If $x_{0}$ is an adherent point of $X ∩ (x_{0}, +∞)$, then we define the right limit $f (x_{0}^{+})$ of $f$ at $x_0$ by the formula $$ \lim_{ x \to x_{0}^{+} }f(x):=\lim_{ x \to x_0:x\in X\cap (x_{0},+\infty) }f(x)   $$ Similarly for the left limit $f(x_{0}^{-})$ of $f$ at $x_{0}$ $$ \lim_{ x \to x_0^{-} }f(x):=\lim_{ x \to x_0:x\in X\cap (-\infty,x_{0}) } f(x)  $$

Notice that only proper limit points of $X$ would be valid choices for $x_0$, as an isolated point would not be adherent to $X\cap(x_{0},+\infty)$ or $X\cap(-\infty,x_{0})$.