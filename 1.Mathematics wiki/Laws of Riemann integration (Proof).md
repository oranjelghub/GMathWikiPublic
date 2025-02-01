---
mathLink: auto
Date created: 2024-07-22 18:47
tags:
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---  

Proved by: [[Laws of integration of the piecewise constant integral]], [[Bounds on the upper and lower Riemann sum]], [[Bounds on the upper and lower Riemann integral]]
References: _Not applicable_
Justifications: [[Riemann integral]], [[Laws of Riemann integration]]  

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote]- Proof: Property 1
> Let $\varepsilon$ be a positive real number, then by definition there exist some majorizing piecewise constant functions $\overline{f}$ and $\overline{g}$ such that $$ \int_{I} f\leq \text{p.c.} \int_{I} \overline{f}\leq \int_{I} f+\varepsilon \land \int_{I} g\leq \text{p.c.} \int_{I} \overline{g}\leq \int_{I} g+\varepsilon $$Then we have $$ \overline {\int}_{I} f+g\leq \text{p.c.} \int_{I} f+g\leq \int_{I} f+\int_{I} g+2\varepsilon $$More generally $$ \int_{I} f+\int_{I} g-2\varepsilon\leq \underline {\int}_{I} f+g\leq \overline {\int}_{I} f+g\leq \int_{I} f+\int_{I} g+2\varepsilon  $$In other words $$ \left| \underline {\int}_{I} f+g-\left( \int_{I} f+\int_{I} g  \right)   \right|\leq 2\varepsilon \land \left| \overline {\int}_{I} f+g-\left( \int_{I} f+\int_{I} g  \right)   \right|\leq 2\varepsilon $$And since $\varepsilon$ is arbitrary we have $$ \underline {\int}_{I} f+g=\overline {\int}_{I} f+g \land \int_{I} f+g=\int_{I} f+\int_{I} g  $$
> 
> **Q.E.D.**

>[!quote]- Proof: Property 2
>The case $c=0$ is trivial so first assume that $c>0$, then if we fix some positive real $\varepsilon$ there exists some majorizing piecewise constant function $\overline{f}$ such that $$ \int_{I} f\leq \text{p.c.} \int_{I} \overline{f}\leq \int_{I} f+\varepsilon $$Since $c\overline{f}$ majorizes $cf$ as well we have that $$ \overline {\int}_{I} cf\leq \text{p.c.} \int_{I} c\overline{f}\leq c\int_{I} f+c\varepsilon $$More generally we have $$ c\int_{I} f-c\varepsilon\leq \underline {\int}_{I} cf\leq  \overline {\int}_{I} cf\leq c\int_{I} f+c\varepsilon  $$Implying $$ \left| c\int_{_{I}} f-\underline {\int}_{I} cf \right| \leq c\varepsilon \land\left| c\int_{_{I}} f-\overline {\int}_{I} cf \right| \leq c\varepsilon $$Meaning that $$ \underline {\int}_{I} cf=\overline {\int}_{I} cf\land \int_{I}  cf=c\int_{I} f $$Now assume that $c=-1$ and fix some $\varepsilon$, then there is some minorizing piecewise constant function $\underline{f}$ such that $$ \int_{I} f-\varepsilon\leq \text{p.c.} \int_{I} \underline{f}\leq \int_{I} f $$Notice that $-\underline{f}$ majorizes $f$ and thus $$ \overline {\int}_{I}  -f\leq \text{p.c.} \int_{I} -\underline{f}\leq -\int_{I} f+\varepsilon $$More generally $$ -\int_{I} f-\varepsilon\leq \underline {\int}_{I} -f\leq \overline {\int}_{I} -f\leq -\int_{I} f+\varepsilon $$Implying $$ \left| \int_{_{I}} f+\underline {\int}_{I} -f \right| \leq \varepsilon \land\left| \int_{_{I}} f+\overline {\int}_{I} -f \right| \leq \varepsilon $$Meaning that $$ \underline {\int}_{I} -f=\overline {\int}_{I} -f\land \int_{I}  -f=-\int_{I} f $$The last case $c<0$ follows from the fact that $c=-1\times-c$ and we can thus apply the previous two cases.
>
>**Q.E.D.**

>[!quote]- Proof: Property 3
>Let $h(x):=f(x)-g(x)$, then $h(x)\geq 0$ for all $x\in I$. Let $\overline{h}$ be a piecewise constant function on $I$ majorizing $h$, then $\overline{h}(x)\geq 0$ for all $x\in I$ and$$ 0\leq \text{p.c.} \int_{I} \overline{h} $$Taking the infimum in $\overline{h}$ gives us $$ 0\leq \int_{I} f-g=\int_{I} f-\int_{I} g $$Meaning that $$ \int_{I} g\leq \int_{I}f  $$
>
>**Q.E.D.**

>[!quote]- Proof: Property 4
>Let $\overline{f}$ be a piecewise constant function on $I$ majorizing $f$, notice that the extension $\overline{F}$ define as $$ \overline{F}(x):=\left\{\begin{align} & \overline{f}(x)&\hspace{1cm} &x\in I\\ &0&\hspace{1cm} &x\not\in I\end{align}  \right.  $$is piecewise constant om $J$ and majorizes $F$, then $$ \overline {\int}_{J} F\leq \text{p.c.} \int_{J} \overline{F}= \text{p.c.} \int_{I} \overline{f} $$Taking the infimum over $\overline{f}$ get us $$ \overline {\int}_{J} F\leq \int_{I} f $$And similarly $$ \int_{I} f\leq \underline {\int}_{J} F $$Thus $F$ is Riemann integrable over $J$ and $$ \int_{J} F=\int_{I} f $$
>
>**Q.E.D.**

>[!quote]- Proof: Property 5
>If we assume that $f|_{J}$ and $f|_{K}$ are Riemann integrable then the result follows, since $$ f=F_{J}+F_{K} $$Where $F_{K}$ and $F_{J}$ are defined as described in property 4. Thus $$ \int_{I} f=\int_{I} F_{J}+F_{K}=\int_{I} F_{J}+\int_{I} F_{K} $$Which by the previous property means that $$ \int_{I} f=\int_{J} f|_{J}+\int_{K} f|_{K} $$To close the proof we now show that indeed $f|_{J}$ and $f|_{K}$ are Riemann integrable. Fix some $\varepsilon$ and let $\overline{f}$,$\underline{f}$ be piecewise constant functions over $I$ satisfying $$ \int_{I} f-\varepsilon\leq \text{p.c.} \int_{I} \underline{f}\leq \int_{I}f\leq \text{p.c.} \int_{I} \overline{f}\leq \int_{I} f+\varepsilon  $$From properties regarding piecewise constant integrals we have $$  \int_{I} f-\varepsilon\leq \text{p.c.} \int_{J} \underline{f}|_{J}+\text{p.c.} \int_{K} \underline{f}|_{K}\leq \int_{I}f\leq \text{p.c.} \int_{J} \overline{f}|_{J}+\text{p.c.} \int_{K} \overline{f}|_{K}\leq \int_{I} f+\varepsilon   $$Implying that $$ 0\leq \left( \text{p.c.} \int_{J} \overline{f}|_{J}+\text{p.c.} \int_{K} \overline{f}|_{K} \right) -\left( \text{p.c.} \int_{J} \underline{f}|_{J}+\text{p.c.} \int_{K} \underline{f}|_{K} \right)\leq 2\varepsilon  $$Or better $$ 0\leq \left( \text{p.c.} \int_{J} \overline{f}|_{J}-\text{p.c.} \int_{J} \underline{f}|_{J} \right)  +\left( \text{p.c.} \int_{K} \overline{f}|_{K} -\text{p.c.} \int_{K} \underline{f}|_{K} \right)\leq 2\varepsilon $$Notice that each of the terms of the sum is positive, thus $$ \begin{align} 0\leq\text{p.c.} \int_{J} \overline{f}|_{J}-\text{p.c.} \int_{J} \underline{f}|_{J} \leq 2\varepsilon \\ 0\leq \text{p.c.} \int_{K} \overline{f}|_{K} -\text{p.c.} \int_{K} \underline{f}|_{K}\leq 2\varepsilon  \end{align} $$But then clearly $$ \begin{align}0\leq \underline {\int}_{J} f|_{J}-\overline {\int}_{J} f|_{J}\leq 2\varepsilon \\ 0\leq \underline {\int}_{K} f|_{K}-\overline {\int}_{K} f|_{K}\leq 2\varepsilon \end{align}$$And since $\varepsilon$ is arbitrary we know that $f|_{J}$ and $f|_{K}$ are both Riemann integrable.
>
>**Q.E.D.**

