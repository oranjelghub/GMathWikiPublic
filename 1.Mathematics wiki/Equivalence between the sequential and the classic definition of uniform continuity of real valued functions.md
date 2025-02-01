---
mathLink: auto
Date created: 2024-06-16 23:06
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Axiom of choice]]
References: _Not applicable_
Justifications: [[Cauchy sequences]], [[Uniform continuity of real valued functions]], [[Sequential definition of uniform continuity of real valued functions]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Equivalence between the sequential and the classic definition of uniform continuity of real valued functions
> Let $X\subseteq \mathbb{R}$ and $f:X\to \mathbb{R}$ a function. Then $f$ is uniformly continuous on $X$ by the classic definition if and only it is uniformly continuous on $X$ by the sequential definition.

>[!quote] Proof: Equivalence between the sequential and the classic definition of uniform continuity of real valued functions
>First suppose that $f$ is uniformly continuous on $X$ by the classic definition. Then for $$ \forall \varepsilon>0\; \exists \delta>0: \forall x,y\in X,\; \left| x-y \right| \leq \delta \implies \left| f(x)-f(y) \right| \leq \varepsilon $$ Given two equivalent sequences $(x_n)^\infty_{n=0}$ and $(y_n)^\infty_{n=0}$ we can make them $\delta$ close because they are equivalent. This would mean that $$ \forall n\geq N, \left| x_{n}-y_{n} \right| \leq \delta \implies \left| f(x_{n})-f(y_{n}) \right| \leq \varepsilon$$ But this directly implies that equivalence of $(f(x_{n}))^\infty_{n=0}$ and $(f(y_{n}))^\infty_{n=0}$, but since the choice of sequences was arbitrary we must have that $f$ is also uniformly continuous on $X$ by the sequential definition. Secondly we prove it the other way around, so suppose $f$ is uniformly continuous on $X$ by the sequential definition, we want to show that $f$ is uniformly continuous on $X$ by the classic definition. To do this, assume for the sake of contradiction that $f$ is not uniformly continuous on $X$ by the classic definition. Then $$ \exists \varepsilon_{\mu}:\forall \delta \exists x_{\mu},y_{\mu}\in X: \left| x_{\mu}-y_{\mu} \right| \leq \delta \land \left| f(x_{\mu})-f(y_{\mu})  \right|>\varepsilon_{\mu}  $$ Then define $$ E_{M}:= \left\{  x,y\in X: \left| x-y \right| \leq \frac{1}{M} \land \left| f(x)-f(y) \right|>\varepsilon_{\mu}   \right\} $$ Which is always non-empty by our assumption. We then pick two choice functions $c_{n}$ and $c'_{n}$ on $\bigcup_{M=1}^\infty E_{M}$, notice that these sequences are equivalent since $\left| c_{M}-c'_{M} \right|\leq \frac{1}{M}$ but there images $f(c_{n})$ and $f(c'_{n})$ are not since for all $M$ we have $\left| f(c_{M}) -f(c'_{M})\right|>\varepsilon_{\mu}$. This contradicts the uniform continuity on $X$ of $f$ by the sequential definition, thus the assumption that $f$ isn't uniformly continuous by the classic definition must be wrong. This prove sthe equivalence of both definitions.
>
>**Q.E.D.**


