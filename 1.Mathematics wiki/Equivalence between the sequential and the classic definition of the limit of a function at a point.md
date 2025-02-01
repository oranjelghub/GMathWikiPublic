---
mathLink: auto
Date created: 2024-05-16 16:21
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Sequential definition of limit of a function at a point]], [[Limit of a real valued function at a point]], [[Axiom of choice]]
References: _Not applicable_
Justifications: [[Convergence of sequences]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Equivalence between the sequential and the classic definition of the limit of a function at a point
> A function $f$ converges $L$ at $x_0$ by the classic definition iff it does by the sequential definition.

>[!quote] Proof: Equivalence between the sequential and the classic definition of the limit of a function at a point
>We first prove the statement from right to left. By the classic definition we have that $$ \forall \varepsilon >0 \exists \delta >0:  x\in \{ y\in E: \left| y-x_{0} \right| \leq \delta \}\implies \left| f(x)-L \right| \leq \varepsilon $$
>Taking some arbitrary sequence of elements of $E$ such that it converges to $x_0$ we know that there exists some $N$ such that for all $n\geq N$ we have $\left| a_{n}-x_{0} \right|\leq \delta$, which means that we have $\left| f(a_{n})-L \right|\leq \varepsilon$. And since $\varepsilon$ is arbitrary we have that $\lim_{ n \to \infty }f(a_{n})=L$. This closes the first implication. Now we proof from left to right. We proceed by contradiction. Suppose that $f$ converges to $L$ by the sequential definition but not the classic one, then we have $$ \exists \varepsilon_{\mu}>0: \forall \delta>0 \;\exists x\in \{ y\in E: \left| y-x_{0} \right|\leq \delta  \}: \left| f(x)-L \right| >\varepsilon_{\mu} $$ Then we can define some non-empty sets $E_{N}:=\left\{  x\in E: \left| x-x_{0} \right|\leq \frac{1}{N}\land \left| f(x)-L \right|>\varepsilon_{\mu}  \right\}$ And define some choice function $(c_n)^\infty_{n=0}$ on $\bigcup_{n\in \mathbb{N}}E_{n}$. Notice that $\lim_{ n \to \infty }c_{n}=x_{0}$ and that by the sequential definition we then must have that $\lim_{ n \to \infty }f(c_{n})=L$, but that's impossible since for all $n\in \mathbb{N}$ we have that $\varepsilon_{\mu}<\left| f(c_{n})-L \right|$. Thus our assumption that the function does not converge to $L$ at $x_{0}$ in $E$ by the classic definition must be wrong.
>
>**Q.E.D.**

