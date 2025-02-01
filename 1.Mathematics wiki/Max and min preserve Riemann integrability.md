---
mathLink: auto
Date created: 2024-07-27 14:03
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Laws of integration of the piecewise constant integral]]
References: _Not applicable_
Justifications: [[Riemann integral]]   

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Max and min preserve Riemann integrability
> Let $I$ be a bounded interval and let $f:I\to \mathbb{R}$ and $g:I\to \mathbb{R}$ be Riemann integrable on $I$. Then $\max(f,g):I\to \mathbb{R}$ and $\min(f,g):I\to \mathbb{R}$ are also Riemann integrable.

>[!quote] Proof: Max and min preserve Riemann integrability
>We only prove that $\max(f,g)$ is Riemann integrable as the proof for $\min(f,g)$ is symmetric. Fix some arbitrary $\varepsilon>0$, then for some piecewise constant functions $$ \begin{align}\int_{I} f-\varepsilon\leq \int_{I} \underline{f}\leq \int_{I} f\leq \int_{I} \overline{f}\leq \int_{I} f+\varepsilon\\ \int_{I} g-\varepsilon\leq \int_{I} \underline{g}\leq \int_{I} g\leq \int_{I} \overline{g}\leq \int_{I} g+\varepsilon  \end{align} $$Such that $\underline{f}\leq f\leq\overline{f}$ and $\underline{g}\leq g\leq\overline{g}$. We define $h:=(\overline{f}-\underline{f})+(\overline{g}-\underline{g})$, notice that $$\int_{I} h\leq 4\varepsilon$$On the other hand, $\max(\underline{f},\underline{g})$ is also piecewise constant on $I$ and minorizes $\max(f,g)$, while similarly $\max(\overline{f},\overline{g})$ majorizes $\max(f,g)$ and is also piecewise constant on $I$. Thus $$ \int_{I} \max(\underline{f},\underline{g})\leq \underline {\int}_{I} \max(f,g)\leq \overline {\int}_{I} \max(f,g)\leq \int_{I} \max(\overline{f},\overline{g}) $$And thus $$ 0\leq \underline {\int}_{I} \max(f,g)-\overline {\int}_{I} \max(f,g)\leq \int_{I} \max(\overline{f},\overline{g})-\max(\underline{f},\underline{g})  $$But notice that $\overline{f}=\overline{f}-\underline{f}+\underline{f}\leq \underline{f}+h$ and similarly $\overline{g}\leq \underline{g}+h$, it follows that $$  0\leq \underline {\int}_{I} \max(f,g)-\overline {\int}_{I} \max(f,g)\leq \int_{I} \max(\underline{f}+h,\underline{g}+h)-\max(\underline{f},\underline{g})=\int_{I} h\leq 4\varepsilon  $$And since $\varepsilon$ is arbitrary we know that $\underline {\int}_{I}\max(f,g)=\overline {\int}_{I}\max(f,g)$ and that the function is Riemann integrable.
>
>**Q.E.D.**
