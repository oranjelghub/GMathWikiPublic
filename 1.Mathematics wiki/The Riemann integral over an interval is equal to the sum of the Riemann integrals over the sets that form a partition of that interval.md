---
mathLink: $\int_{I}f=\sum^{}_{J\in P}\int_{J} f$ where $P$ is a partition of $I$
Date created: 2024-07-29 19:17
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Laws of Riemann integration]]
References: _Not applicable_
Justifications: [[Riemann integral]], [[Interval partition of a bounded interval]] 

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: The Riemann integral over an interval is equal to the sum of the Riemann integrals over the sets that form a partition of that interval
> Let $I$ be a bounded interval and $f:I\to \mathbb{R}$ be a Riemann integrable function. If $P$ is a partition of $I$, then $$ \int_{I}f=\sum^{}_{J\in P}\int_{J}f $$

>[!quote] Proof: The Riemann integral over an interval is equal to the sum of the Riemann integrals over the sets that form a partition of that interval
>We proceed by induction on the cardinality of $P$, let $k=0$, then $P_{0}$ is empty and so is $I$. This immediately closes the case since both sides are equal to zero. Now let $P_{n}$ be a partition of cardinality $n$, we may write $P_{n}=\{ I_{i} \}_{1\leq i\leq n}$, and we assume for our inductive hypothesis that $$ \int_{I} f=\sum^{}_{J\in P_{n}}\int_{J} f $$Now we wan to show this holds for some partition $P_{n+1}$. Since $I$ is bounded it has some finite right end point $b$, if $P_{n+1}$ is a partition of $I$ we must have some interval in $P_{n+1}$ that has $b$ as right end point as well (this can be proven by contradiction pretty easily). Without loss of generality assume that the set in question is exactly $I_{n+1}$, then $I\backslash I_{n+1}$ is also a interval, and we have that $\{ P_{n+1}\backslash I_{n+1}, I_{n+1} \}$ forms a partition of $I$, implying that $$ \int_{I} f=\int_{P_{n+1}\backslash I_{n+1}} f+\int_{I_{n+1}} f $$Which by the inductive hypothesis is equal to $$ \int_{I} f= \sum^{}_{J\in P_{n+1}\backslash I_{n+1}}\int_{J} f+\sum^{ }_{J\in \{ I_{n+1} \}}\int_{J} f $$Which by laws of summations means $$ \int_{I} f= \sum^{}_{J\in P_{n+1} }\int_{J} f $$Which closes the induction.
>
>**Q.E.D.**