---
mathLink: Discontinuity of the Stieltjes-$\mathbb{Q}$ function on $\mathbb{Q}$
Date created: 2024-09-20 19:12
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Interspersing of reals by rationals]]
References: _Not applicable_
Justifications: [[Stieltjes-Q function]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Discontinuity of the Stieltjes-$\mathbb{Q}$ function on $\mathbb{Q}$
>  Let $\Xi_{\mathbb{Q}}$ be the Stieltjes-$\mathbb{Q}$ function with respect to some arbitrary bijective sequence $(q_n)^\infty_{n=0}$ which maps $\mathbb{N}\to \mathbb{Q}$. Then $\Xi_{\mathbb{Q}}$ is discontinuous on $\mathbb{Q}$.

>[!quote] Proof: Discontinuity of the Stieltjes-$\mathbb{Q}$ function on $\mathbb{Q}$
>Let $p\in \mathbb{Q}$, since $p$ is rational we have that $p=q_n$ for some $n\in \mathbb N$. Since between two real numbers there always exists some rational number, we know that there is some $p'$ such that $p<p'<x$ for all $x\in \mathbb R_{>p}$. By the monotonicty of $f$ we get that $$\sum_{r\in \mathbb Q: r<p}g(r)\leq \sum_{r\in \mathbb Q: r<p'}g(r)\leq \sum_{r\in \mathbb Q: r<x}g(r)$$This implies that $$\sum_{r\in \mathbb Q: r<p}g(r)+2^{-n}\leq \sum_{r\in \mathbb Q: r<x}g(r)$$In other words for all $x>p$, the following inequality always holds $$f(x)\geq f(p)+2^{-n}$$Notice that this means that if we fix $\varepsilon:= 2^{-(n+1)}$, no matter the choice of $\delta>0$ we will always have that $$x>p \land |x-p|\leq \delta \implies |f(x)-f(p)|>\varepsilon$$In other words, $f$ is discontinuous at $p$, or more generally, $f$ is discontinuous on $\mathbb Q$.
>
>**Q.E.D.**


