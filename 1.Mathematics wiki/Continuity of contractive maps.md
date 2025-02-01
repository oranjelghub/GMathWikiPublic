---
mathLink: auto
Date created: 2024-05-25 20:57
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: _Not applicable_
References: _Not applicable_
Justifications: [[Continuity (Metric space)]], [[Contractions]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Continuity of contractive maps
> Let $(X,d)$ be a metric space and $\Phi$ a contraction on $X$. Then $\Phi$ is a continuous map.

>[!quote] Proof: Continuity of contractive maps
>Fix some $\varepsilon>0$, we want to find a $\delta>0$ such that $$\forall x,y\in X, d(x,y)\leq \delta\implies d(\Phi(x),\Phi(y))\leq \varepsilon$$ Fixing $\varepsilon=\delta$ gives us $$ \forall x,y\in X, d(\Phi(x),\Phi(y))\leq qd(x,y)\leq d(x,y)\leq \varepsilon $$ Thus $\Phi$ is a continuous map.
>
>**Q.E.D.**


