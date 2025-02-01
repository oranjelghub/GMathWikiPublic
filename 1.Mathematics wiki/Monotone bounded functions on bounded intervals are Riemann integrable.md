---
mathLink: auto
Date created: 2024-08-01 17:20
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Monotone real valued functions on (a,b) are Riemann integrable]]
References: _Not applicable_
Justifications: [[Riemann integral]], [[Piecewise constant integral]]   
   

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Monotone bounded functions on bounded intervals are Riemann integrable
> Let $I$ be a bounded interval, and let $f:I\to \mathbb{R}$ be both monotone and bounded, then $f$ is Riemann integrable.

>[!quote] Proof: Monotone bounded functions on bounded intervals are Riemann integrable
>The claim follows by a previous result if $I$ is closed, or it trivially follows if $I$ is empty or a singleton. So assume it has endpoints $a<b$. Fix some $\varepsilon$ such that $0\leq \varepsilon< \frac{b-a}{2}$ and notice that $f$ is Riemann integrable on $[a+\varepsilon,b-\varepsilon]$ since it's a closed interval and $f$ is still monotone there. We know that for some piecewise constant function $h$ that majorizes $f$ that $$ \int_{[a+\varepsilon,b-\varepsilon]} h\leq \int_{[a+\varepsilon,b-\varepsilon]} f+\varepsilon $$Defining $\tilde{h}$ as: $\tilde{h}(x):=h(x)$ if $x\in[a+\varepsilon,b-\varepsilon]$ and $\tilde{h}(x):=M$ otherwise, where $M$ is a bound of $f$. Then $$  \int_{[a+\varepsilon,b-\varepsilon]} h+2M\varepsilon\leq \int_{[a+\varepsilon,b-\varepsilon]} f+(2M+1)\varepsilon  $$Implying $$ \int_{I} \tilde{h}\leq  \int_{[a+\varepsilon,b-\varepsilon]} f+(2M+1)\varepsilon $$More generally, and by reproducing the argument for some minorizing piecewise constant function $$ 0\leq \overline {\int}_{I} f-\underline {\int}_{I} f\leq (4M+2)\varepsilon   $$Since the choice of $\varepsilon$ is arbitrary we must have that $f$ is Riemann integrable on $I$.

