---
mathLink: $\alpha$-length of intervals
Date created: 2024-08-04 16:59
tags:
  - Type/Object
  - Topic/Real_Analysis
cssclasses:
---

---  

Types: Examples: _Not applicable_
Examples: _Not applicable_
Construction: [[Piecewise constant Riemann-Stieltjes integral]]
Generalization: [[Measure]]

Properties: [[Alpha-length is finitely additive]]
Sufficiencies: _Not applicable_
Equivalences: _Not applicable_
Justifications: [[Limit of a real valued function at a point]], [[Alpha-length of intervals are well-defined]]

---

> [!quote] Definition: $\alpha$-length of intervals
> Let $X\subset \mathbb{R}$ be a closed interval and let $\alpha:X\to \mathbb{R}$ be a monotone increasing function. Let $I\subseteq X$ be a bounded interval, then we define the $\alpha$-length $\alpha[I]$ by the following rules
> 1. If $I=\emptyset$, then $\alpha[I]:=0$
> 2. If $I=\{ a \}$, then $\alpha[I]:= \lim_{ x \to a^{+}:x\in X }\alpha(x)-\lim_{ x \to a^{-}:x\in X }\alpha(x)$. With the convention that if $a$ is the right-endpoint of $X$ (resp. left-endpoint) then $\lim_{ x \to a^{+}:x\in X }\alpha(x)$ (resp. $\lim_{ x \to a^{-}:x\in X }\alpha(x)$) is equal to $\alpha(a)$
> 3. If $I=(a,b)$, then $\alpha[I]:=\lim_{ x \to b^{-}:x\in X }\alpha(x)-\lim_{ x \to a^{+}:x\in X }\alpha(x)$
> 4. If $I$ is equal to $(a,b]$, $[a,b)$, or $[a,b]$, then $\alpha[I]:=\alpha[(a,b)]+\alpha[\{ b \}]$, $\alpha[I]:= \alpha[\{ a \}]+\alpha[(a,b)]$, or $\alpha[I]:= \alpha[\{ a \}]+\alpha[(a,b)]+\alpha[\{ b \}]$

Although this definition may seem complicated, notice that if $\alpha$ is continuous on $X$ that $$ \alpha[I]=\alpha(b)-\alpha(a) $$Whenever $a\leq b$ are the endpoints of $I$. Notice also that we have $\alpha[I]\geq 0$ for all $I$. In some sense we defined a arbitrary [[Measure]] on the intervals, although this formally can't be called a [[Measure]] since we don't have a proper associated [[Sigma-algebra]]

