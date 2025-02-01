---
mathLink: auto
Date created: 2024-06-12 19:33
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Intermediate value theorem]]
References: _Not applicable_
Justifications: [[Monotone real valued functions]], [[Continuity of real valued functions]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem Continuous injections are monotone
> Let $a<b$ and $f:[a,b]\to \mathbb{R}$ be a continuous injection on $[a,b]$, then $f$ is strictly monotone.

>[!quote] Proof: Continuous injections are monotone
>We know that either $f(a)<f(b)$ or $f(a)=f(b)$ or $f(a)>f(b)$. $f(a)=f(b)$ is obviously wrong as it would contradict the injectivity of $f$, so we know either $f(a)<f(b)$ or $f(a)>f(b)$. WLOG assume that $f(a)<f(b)$, we claim that for any $c$ satisfying $a<c<b$ we have $f(a)<f(c)<f(b)$. We prove this by contradiction, so assume that $f(a)<f(b)<f(c)$ (the case for $f(c)<f(a)<f(b)$ is symmetric). Notice that since both restrictions $f|_{[a,c]}$ and $f|_{[c,b]}$ are continuous we can fix some random $y$ which satisfies $f(a)<f(b)<y<f(c)$ and use the intermediate value theorem to conclude that there exists a $k\in [a,c]$ such that $f(k)=y$ and a $k'\in [c,b]$ such that $f(k')=y$, but since $k\neq k'$ we have a contradiction since $f$ is supposed to be injective. So the assumption that $f(a)<f(b)<f(c)$ must be wrong and we must have that $f(a)<f(c)<f(b)$, in other words $f$ is strictly monotone (increasing in this case). 
>
>**Q.E.D.**