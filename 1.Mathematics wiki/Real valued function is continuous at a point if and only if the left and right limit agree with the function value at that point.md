---
mathLink: auto
Date created: 2024-05-25 17:07
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: _Not applicable_
References: _Not applicable_
Justifications: [[Continuity of real valued functions]], [[Left and right limits of real valued functions]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Real valued function is continuous at a point if and only if the left and right limit agree
> Let $X$ be a subset of $\mathbb{R}$ containing a real number $x_0$, and suppose that $x_{0}$ is an adherent point of both $X ∩ (x_{0}, +∞)$ and $X ∩ (−∞, x_{0})$. Let $f : X → \mathbb{R}$ be a function. If $\lim_{ x \to x_{0}^{+} }f(x)$ and $\lim_{ x \to x_{0}^{-} }f(x)$ both exist and are both equal to $f (x_{0})$, then $f$ is continuous at $x_0$.

>[!quote] Proof: Real valued function is continuous at a point if and only if the left and right limit agree
>Suppose that $\lim_{ x \to x_0:x\in X }f(x)=f(x_{0})$, then every sequence $(a_n)^\infty_{n=0}$ made of elements of $X$ that converges to $x_{0}$ induces some convergent sequence $(f(a_n))^\infty_{n=0}$ that converges to $f(x_{0})$, but more specifically this also holds if the sequence only contains elements of $X \cap (x_{0},+\infty)$ or $X\cap(-\infty,x_{0})$ . Thus this implies that the left and right limits agree and that both ar equal to $f(x_{0})$. Now suppose that the left and right limit agree and that they both converge to $f(x_{0})$. This means that $$ \begin{align} \forall \varepsilon \exists \delta_{+}: \forall x\in X \cap (x_{0},+\infty), \left| x-x_{0} \right| \leq \delta_{+}\implies \left| f(x)-f(x_{0}) \right| \leq \varepsilon \\  \forall \varepsilon \exists \delta_{-}: \forall x\in X \cap (-\infty,x_{0}), \left| x-x_{0} \right| \leq \delta_{-}\implies \left| f(x)-f(x_{0}) \right| \leq \varepsilon\end{align} $$ But notice that this implies that $$ \forall x\in X, \left| x-x_{0} \right| \leq \min(\delta_{+},\delta_{-})\implies \left| f(x)-f(x_{0}) \right|\leq \varepsilon  $$ Meaning that indeed $\lim_{ x \to x_0:x\in X }f(x)=f(x_{0})$.
>
>**Q.E.D.**
