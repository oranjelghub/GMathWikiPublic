---
mathLink: Monotone real valued functions on $[a,b]$ are Riemann integrable
Date created: 2024-08-01 16:54
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Telescoping series]]
References: _Not applicable_
Justifications: [[Riemann sums]], [[Riemann integral]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Monotone real valued functions on $[a,b]$ are Riemann integrable
> Let $a<b$ be real and let $f:[a,b]\to \mathbb{R}$ be a monotone function. Then $f$ is Riemann integrable.

>[!quote] Proof: Monotone real valued functions on $[a,b]$ are Riemann integrable
>WLG suppose that $f$ is monotone increasing, then we know that $f$ is bounded since $f(x)\leq f(b)$ for all $x\in [a,b]$. Now fix some integer $N>0$, and define the partition $$ P:=  \left\{ [a+ \frac{b-a}{N}j,a+\frac{b-a}{N}(j+1)): 0\leq j\leq N-1 \right\}\cup \{ b \}  $$Then we can consider the upper Riemann sum, and specifically have $$ \overline {\int}_{I} f\leq \sum^{N-1}_{j=0} \left( \sup_{x\in[a+ \frac{b-a}{N}j,a+\frac{b-a}{N}(j+1))} f(x) \right)  \frac{b-a}{N} $$And since $f$ is monotone increasing $$ \overline {\int}_{I} f\leq \sum^{N-1}_{j=0}f\left( a+ \frac{b-a}{N}(j+1) \right) \frac{b-a}{N} $$Doing the same for the lower Riemann sum grants us $$ \overline {\int}_{I} f-\underline {\int}_{I} f\leq\sum^{N-1}_{j=0}\left( f\left( a+ \frac{b-a}{N}(j+1) \right)-f\left( a+ \frac{b-a}{N}j  \right) \right)  \frac{b-a}{N}  $$But this is just a simple telescoping series that can be reduced to $$\overline {\int}_{I} f-\underline {\int}_{I} f\leq \frac{(f(b)-f(a))(b-a)}{N}$$But since $N$ was arbitrary, we must have that $f$ is Riemann integrable.
>
>**Q.E.D.**

