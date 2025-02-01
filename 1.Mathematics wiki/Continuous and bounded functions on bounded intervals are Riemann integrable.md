---
mathLink: auto
Date created: 2024-07-30 17:15
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Continuous function on (a,b) are Riemann integrable]]
References: _Not applicable_
Justifications: [[Riemann integral]], [[Piecewise constant integral]]   

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Continuous and bounded functions on bounded intervals are Riemann integrable
> Let $I$ be a bounded interval and $f:I\to \mathbb{R}$ be a continuous and bounded function. Then $f$ is Riemann integrable on $I$. 

>[!quote] Proof: Continuous and bounded functions on bounded intervals are Riemann integrable
>The claim follows by a previous result if $I$ is closed, or it trivially follows if $I$ is empty or a singleton. So assume it has endpoints $a<b$. Fix some $\varepsilon$ such that $0\leq \varepsilon< \frac{b-a}{2}$ and notice that $f$ is Riemann integrable on $[a+\varepsilon,b-\varepsilon]$ since $f$ is continuous there and it is a closed interval. We know that for some piecewise constant function $h$ that majorizes $f$ that $$ \int_{[a+\varepsilon,b-\varepsilon]} h\leq \int_{[a+\varepsilon,b-\varepsilon]} f+\varepsilon $$Defining $\tilde{h}$ as: $\tilde{h}(x):=h(x)$ if $x\in[a+\varepsilon,b-\varepsilon]$ and $\tilde{h}(x):=M$ otherwise, where $M$ is a bound of $f$. Then $$  \int_{[a+\varepsilon,b-\varepsilon]} h+2M\varepsilon\leq \int_{[a+\varepsilon,b-\varepsilon]} f+(2M+1)\varepsilon  $$Implying $$ \int_{I} \tilde{h}\leq  \int_{[a+\varepsilon,b-\varepsilon]} f+(2M+1)\varepsilon $$More generally, and by reproducing the argument for some minorizing piecewise constant function $$ 0\leq \overline {\int}_{I} f-\underline {\int}_{I} f\leq (4M+2)\varepsilon   $$Since the choice of $\varepsilon$ is arbitrary we must have that $f$ is Riemann integrable on $I$.
>
**Q.E.D.**



