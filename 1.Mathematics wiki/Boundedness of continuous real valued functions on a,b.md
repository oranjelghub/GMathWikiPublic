---
mathLink: Boundedness of continuous real valued functions on [a,b]
Date created: 2024-05-27 14:14
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Axiom of choice]], [[Heine-Borel theorem for the real line]]
References: _Not applicable_
Justifications: [[Sequential definition of continuity of real valued functions]], [[Equivalence between the sequential and the classic definition of continuity of real valued functions]]

Specializations: _Not applicable_
Generalizations: [[Maximum principle for real valued functions]]

---

> [!quote] Theorem: Boundedness of continuous real valued functions on $[a,b]$
> Let $a<b$ be real numbers and let $f:[a,b]\to \mathbb{R}$ be a continuous function on $[a,b]$. Then $f$ is bounded.

>[!quote] Proof: Boundedness of continuous real valued functions on $[a,b]$
>We proceed by contradiction, suppose $f$ was not bounded. Then the set $$ E_{M}:=\{ x\in [a,b]: \left| f(x) \right| >M  \} $$ is never non-empty. Thus we can define some choice function $(c_n)^\infty_{M=0}$ on $\bigcup_{M\in \mathbb{N}}E_{M}$. Now notice that we have $f(c_{N})>N$. Since $[a,b]$ is closed and bounded we know that according to the Heine-Borel theorem there exists some subsequence $(c_{\sigma(m)})^\infty_{m=0}$ such that $\lim_{ m \to \infty }c_{\sigma(m)}=L\in [a,b]$. But since $f$ is continuous notice that we have $$ \begin{align} \lim_{ m \to \infty }f(c_{\sigma(m)} ) &= f(L)\end{align} $$ In other words $f(c_{\sigma(m)})$ is a convergent sequence, but this isn't possible since $$ M<\sigma(M)<f(c_{\sigma(M)}) $$ Thus our original assumption must be false and $f$ must be bounded.
>
>**Q.E.D.**


