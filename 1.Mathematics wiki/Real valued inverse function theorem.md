---
mathLink: auto
Date created: 2024-07-11 21:54
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Sequential definition of limit of a function at a point]], [[Algebra of sequence limits]]
References: _Not applicable_
Justifications: [[Inverse functions]], [[Differentiation of real valued functions]], [[Continuity of real valued functions]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---



> [!quote] Theorem: Real valued inverse function theorem
> Let $X,Y\subseteq \mathbb{R}$, and let $f:X\to Y$ be an invertible function. Suppose that $x_{0}\in X$ and $y_{0}\in Y$ are limit points of $X$,$Y$, respectively, such that $f(x_{0})=y_{0}$. If $f$ is differentiable at $x_{0}$ with non-zero derivative and $f^{-1}$ is continuous at $y_{0}$ then $f^{-1}$ is differentiable at $y_{0}$ and $$ \left( f^{-1} \right) '(y_{0})=\frac{1}{f'(x_{0})} $$

>[!quote] Proof: Real valued inverse function theorem
>We want to show that $$ \lim_{ y \to y_{0}:y\in Y\backslash\{ y_{0} \} } \frac{f^{-1}(y)-f^{-1}(y_{0})}{y-y_{0}}=\frac{1}{f'(x_{0})} $$By the sequential limit definition it suffices to show that $$ \lim_{ n \to \infty } \frac{f^{-1}(y_{n})-f^{-1}(y_{0})}{y_{n}-y_{0}}=\frac{1}{f'(x_{0})} $$For any sequence $(y_n)^\infty_{n=1}$ that converges to $y_{0}$ and is made of elements of $Y\backslash\{ y_{0} \}$. To prove this we define $x_{n}:=f^{-1}(y_{n})$, which we notice is a sequence of elements of $X\backslash\{ x_{0} \}$. Since $f^{-1}$ is continuous by assumption we notice that $\lim_{ n \to \infty }x_{n}=\lim_{ n \to \infty }f^{-1}(y_{n})=f^{-1}(y_{0})=x_{0}$, and since $f$ is differentiable at $x_{0}$ we have that $$ \lim_{ n \to \infty } \frac{f(x_{n})-f(x_{0})}{x_{n}-x_{0}}=f'(x_{0}) $$By hypothesis $f'(x_{0})$ is non-zero and so is $\frac{f(x_{n})-f(x_{0})}{x_{n}-x_{0}}$ for every $n$, thus we may invert both expressions to get $$ \frac{1}{f'(x_{0})}=\lim_{ n \to \infty } \frac{x_{n}-x_{0}}{f(x_{n})-f(x_{0})} $$Which by definition is equal to $$ \frac{1}{f'(x_{0})}=\lim_{ n \to \infty } \frac{f^{-1}(y_{n})-f^{-1}(y_{0})}{y_{n}-y_{0}} $$ As desired.
>
>**Q.E.D.**

