---
Date created: 2024-09-29 12:26
tags:
  - Type/Refined_Note
  - Topic/Physics
---

---

Types: _Not applicable_
Examples: _Not applicable_
Properties: _Not applicable_

Justifications: [[Center of mass in a discrete system]], [[Center of mass in a continuous 3 dimensional system with uniform density]]
Specializations: _Not applicable_
Generalization: _Not applicable_

---

Consider the following system with uniform density $\rho$ and radius $R$
![[dEdTNc01.svg#invert_B|300]]
With partition this semi-circle along the drawn $x$-axis, calling the intersection points of the horizontal line with the $x$-axis $x_{j}$. We now want to find the $x$ coordinate, which we note $r_{x}$ of the center of mass of this system. For our discrete partition into $k$ strips the $x$ center of mass is given by $$ r_{x}\approx\frac{\sum^{k}_{j=i} m_{j}x_{j}}{M}$$Note know that every mass $m_{j}$ is equal to $$ m_{j}=2\rho(x_{j}-x_{j-1})l $$Where $l$ is also drawn. We may compute $l$ by considering the following triangle and applying the Pythagorean theorem![[diagram-20240929.svg#invert_B|520]]
Thus $$ m_{j}=2\rho(x_{j}-x_{j-1})\sqrt{ R^{2}-x_{j}^{2} } $$And it follows that for a discrete partition into $k$ strips we have $$  r_{x}\approx\frac{\sum^{k}_{j=i} 2\rho(x_{j}-x_{j-1})\sqrt{ R^{2}-x_{j}^{2} }\;x_{j}}{M} $$Notice that since $x_{j}-x_{j-1}=\Delta x_{j}$, we may now transition to continuous by transforming $\Delta x_{j}\to dx$ and $x_{j}\to x$. We then get $$r_{x}= \frac{2\rho}{M} \int_{0}^{R}x\sqrt{ R^{2}-x^{2} }\; dx  $$We will not solve the integral since it is a pretty standard one, but the solution is $\int_{0}^{R}x\sqrt{ R^{2}-x^{2} }\; dx=\frac{R^{3}}{3}$, also not forgetting that $M=\frac{\pi R^{2}}{2}\rho$, we have $$ r_{x}=\frac{2\rho}{\frac{\pi R^{2}}{2}\rho}*\frac{R^{3}}{3}=\frac{4R}{3\pi} $$Since the shape is symmetrical around the $y$-axis, the center of mass will simply lie on the $x$-axis itself, thus $$ r=\left( \frac{4R}{3\pi},0 \right) $$