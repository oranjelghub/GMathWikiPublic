---
mathLink: auto
Date created: 2024-07-30 16:11
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Uniformly continuous real valued functions preserve boundedness of sets]], [[Archimedean property]]
References: _Not applicable_
Justifications: [[Riemann integral]], [[Upper and lower Riemann integral in terms of Riemann sums]], [[Uniform continuity of real valued functions]]   

Specializations: [[Continuous function on (a,b) are Riemann integrable]]
Generalizations: [[Uniformly continuous functions on bounded intervals are Riemann-Stieltjes integrable]]

---

> [!quote] Theorem: Uniformly continuous functions on bounded intervals are Riemann integrable
> Let $I$ be a bounded interval and $f:I\to \mathbb{R}$ be a functions uniformly continuous on $I$. Then $f$ is Riemann integrable on $I$.

>[!quote] Proof: Uniformly continuous functions on bounded intervals are Riemann integrable
>First of all since $f$ is uniformly continuous we know that $f(I)$ is a bounded set and thus $f$ is bounded. We may assume for the sake of non-triviality that $I$ has endpoints $a<b$. Now fix some arbitrary $\varepsilon>0$, then by uniform continuity $$ \exists \delta>0: \left| x-y \right| \leq \delta \implies \left| f(x)-f(y) \right|\leq \varepsilon  $$And by the Archimedean property $$ \exists N: \frac{b-a}{N}\leq \delta $$We may then make a partition of $I$ into $N$ intervals all of length $\frac{b-a}{N}$ (we will not give a explicit construction as it is trivial). Thus we have the partition $\{ J_{k} \}_{1\leq k\leq N}$ and  $$\sum^{N}_{k=1}(\inf_{x\in J_{k}}f(x))\mu(J_{k})\leq \underline {\int}_{I} f\leq \overline {\int}_{I} f\leq \sum^{N}_{k=1} (\sup_{x\in J_{k}}f(x))\mu(J_{k})$$Implying $$ \overline {\int}_{I} f-\underline {\int}_{I} f\leq \sum^{N}_{k=1}(\inf_{x\in J_{k}}f(x)-\sup_{x\in J_{k}}f(x))\mu(J_{k}) $$For all $x,y \in J_{k}$, we obviously have $\left| x-y \right|\leq \delta$, so by uniform continuity $$ f(x)\leq f(y)+\varepsilon $$Taking the supremum in $f$ on the right side and the infimum on the left side we have $$ \sup_{x\in J_{k}}f(x)\leq \inf_{x\in J_{k}}f(x)+\varepsilon $$It follows that $$ \overline {\int}_{I} f-\underline {\int}_{I} f\leq \sum^{N}_{k=1} \varepsilon \mu(J_{k})=\varepsilon(b-a)$$And since $\varepsilon$ is arbitrary, we have that $f$ is Riemann integrable.
>
>**Q.E.D.**
