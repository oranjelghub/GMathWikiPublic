---
mathLink: auto
Date created: 2024-10-07 10:20
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Rolle's theorem]]
References: _Not applicable_
Justifications: [[Continuity of real valued functions]], [[Differentiation of real valued functions]]

Specializations: [[Mean value theorem]]
Generalizations: _Not applicable_

---

> [!quote] Theorem: Cauchy's mean value theorem
> Let $[a,b]\subseteq \mathbb{R}$ and let $f:[a,b]\to \mathbb{R}$ and $g:\to \mathbb{R}$ be continuous on $[a,b]$ and differentiable on $(a,b)$. Then there exists some $c\in (a,b)$ such that $$ (f(b)-f(a))g'(c)=(g(b)-g(a))f'(c) $$

>[!quote] Proof: Cauchy's mean value theorem
>Define the function $$ h(x):=(f(b)-f(a))g(x)-(g(b)-g(a))f(x) $$Defined on $[a,b]$. Notice that $h(a)=h(b)$, and that $h$ is stil continuous on $[a,b]$ and differentiable on $(a,b)$. This means that according to Rolle's theorem that there exists some $c\in (a,b)$ such that $$  (f(b)-f(a))g'(c)-(g(b)-g(a))f'(c)=0$$It follows that $$ (f(b)-f(a))g'(c)=(g(b)-g(a))f'(c) $$
>
>**Q.E.D.**
