---
mathLink: auto
Date created: 2024-07-12 22:57
tags:
  - Type/Theorem
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Newton's approximation]], [[Limit laws for real valued functions]], [[Rolle's theorem]], [[Sequential definition of limit of a function at a point]], [[Axiom of choice]]
References: [[L'Hôpital's rule (Proof)]]
Justifications: [[Continuity of real valued functions]], [[Differentiation of real valued functions]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

We state two different formulations of the theorem, and compare them further down the note.

> [!quote] Theorem: L'Hôpital's rule (I)
> Let $X$ be a subset of $\mathbb{R}$, let $f:X\to \mathbb{R}$ and $g:X\to \mathbb{R}$ be functions, and let $x_{0}\in X$ be a limit point of $X$. Suppose that $f(x_{0})=g(x_{0})=0$, that $f$ and $g$ are both differentiable at $x_{0}$ and that $g'(x_{0})\neq 0$. Then there exists some $\delta>0$ such that $$ \forall x\in \left( X\cap (x_{0}-\delta,x_{0}+\delta) \right)\backslash \{ x_{0} \}, \;g(x)\neq 0  $$and $$ \lim_{ x \to x_0:x\in \left( X\cap (x_{0}-\delta,x_{0}+\delta) \right)\backslash \{ x_{0} \} } \frac{f(x)}{g(x)}= \frac{f'(x_{0})}{g'(x_{0})}  $$

>[!quote] Theorem: L'Hôpital's rule (II)
>Let $a<b$ be real numbers, and let $f:[a,b]\to \mathbb{R}$ and $g:[a,b]\to \mathbb{R}$ which are continuous on $[a,b]$. Let $c\in [a,b]$. Suppose both $f$ and $g$ are differentiable on $[a,b]\backslash\{ c \}$, that $f(c)=g(c)=0$, that $g'$ is non-zero on $[a,b]\backslash\{ c \}$, and $\lim_{ x \to c:x\in [a,b]\backslash\{ c \}} \frac{f'(x)}{g'(x)}$ exists and is equal to $L$. Then $g(x)\neq 0$ for all $x\in [a,b]\backslash\{ c \}$ and $\lim_{ x \to c :x\in [a,b]\backslash\{ c \}} \frac{f(x)}{g(x)}$ exists and is equal to $L$.

We now compare both in a sidenote.

>[!quote]- Sidenote: Comparing the two theorems
>Table of comparison 
>
>|                                                             |                                                                                                                             |
| :---------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------------------------: |
|                           **(I)**                           |                                                          **(II)**                                                           |
|         Works on arbitrary subsets of $\mathbb{R}$          |                                             Works on intervals of $\mathbb{R}$                                              |
| Requires the functions to only be differentiable at $x_{0}$ |              Requires the functions to be continuous on $[a,b]$ and differentiable on $(a,b)\backslash\{ c \}$              |
|    Requires $\frac{f'(x_{0})}{g'(x_{0})}$ to be defined     | Doesn't require $\frac{f'(c)}{g'(c)}$ to be defined, only $\lim_{ x \to c:x\in [a,b]\backslash\{ c \}} \frac{f'(x)}{g'(x)}$ |
|                         Single use                          |                       May be used multiple times in a row, where the last use can instead be **(I)**                        | 









