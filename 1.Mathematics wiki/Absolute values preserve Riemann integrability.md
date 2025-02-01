---
mathLink: auto
Date created: 2024-07-27 14:29
tags:
  - Type/Theorem
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Max and min preserve Riemann integrability]]
References: _Not applicable_
Justifications: [[Riemann integral]]  

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Absolute values preserve Riemann integrability
> Let $I$ be a bounded interval and let $f:I\to \mathbb{R}$ be a Riemann integrable function on $I$. Then $\left| f \right|$ is also Riemann integrable on $I$.

The proof follows directly from the fact that we can write $$ \left| f \right| =\max(f,0)+\min(f,0) $$And since min and max operators preserve Riemann integrability we know that $\left| f \right|$ is Riemann integrable on $I$.