---
mathLink: auto
Date created: 2024-07-10 18:30
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Rolle's theorem]]
References: _Not applicable_
Justifications: [[Continuity of real valued functions]], [[Differentiation of real valued functions]], [[Laws of differentiation of real valued functions]], [[Function arithmetic preserves continuity]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Mean value theorem
> Let $a<b$ be real numbers and $f:[a,b]\to \mathbb{R}$ be a function such that $f$ is continuous on $[a,b]$ and differentiable on $(a,b)$. Then there exists some $c\in (a,b)$ such that $$ f'(c)=\frac{f(b)-f(a)}{b-a} $$

>[!quote] Proof: Mean value theorem
>Consider $$ g:[a,b]\to \mathbb{R}: x\mapsto f(x)-Mx $$Where $M:= \frac{f(b)-f(a)}{b-a}$, notice that $g$ is still continuous on $[a,b]$ and differentiable on $(a,b)$ since $-Mx$ is so as well and thus the differentiability and continuity is preserved through function arithmetic. Also, notice that $g(a)=g(b)$, thus we can apply Rolle's theorem to claim that there exists some $c\in (a,b)$ such that $g'(c)=0$, meaning that $$ g'(c)=f'(c)-M=0 \implies f'(c)=M $$Which closes the proof. 
>
>**Q.E.D.**


