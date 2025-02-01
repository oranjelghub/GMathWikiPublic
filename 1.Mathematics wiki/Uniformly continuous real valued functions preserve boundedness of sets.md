---
mathLink: auto
Date created: 2024-06-22 01:32
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Uniformly continuous real valued functions have a limit in every adherent point]], [[Bolzano-Weierstrass theorem]]
References: _Not applicable_
Justifications: [[Sequential definition of limit of a function at a point]], [[Axiom of choice]], [[Uniform continuity of real valued functions]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Uniformly continuous real valued functions preserve boundedness of sets
> Let $X\subseteq \mathbb{R}$ and $f:X\to \mathbb{R}$ a uniformly continuous function on $X$. Let $E\subseteq X$ be a bounded set, then $f(E)$ is bounded.

>[!quote] Proof: Uniformly continuous real valued functions preserve boundedness of sets
>We proceed by contradiction, so assume that $f(E)$ is unbounded. Then $$ A_{M}:=\{ x\in E: x\in f(E)\backslash [-M, M] \}$$ is non-empty for all non-zero $M$ by hypothesis. We can thus pick some choice function $(c_n)^\infty_{n=1}\in \bigcup_{M=1}^{\infty}A_{M}$. Now since $E$ is a bounded set we have that $(c_n)^\infty_{n=1}$ is a bounded sequence, which by  the Bolzano-Weierstrass theorem implies the existence of some convergent subsequence $(c_{\sigma(n)})^\infty_{n=1}$, which has a limit $x_{0}$ in $X$ but not necessarily in $E$. Although, since it's limit is obviously adherent to $E$, at the very least the limit of $f$ at $x_{0}$ must exist. But notice that this is impossible, since if the limit at $x_{0}$ existed and was equal to some real $L$, then for all sequences converging to $x_0$ their sequence of images must converge to $L$. But clearly $\lim_{ n \to \infty }c_{\sigma(n)}=x_{0}$ whilst $(f(c_{\sigma(n)}))^\infty_{n=1}$ is a divergent sequence. Which is a contradiction to the fact that $f$ must have a limit at all the adherent points of $E$. Thus our original assumption that $f(E)$ is unbounded must be wrong.
>
>**Q.E.D.**


