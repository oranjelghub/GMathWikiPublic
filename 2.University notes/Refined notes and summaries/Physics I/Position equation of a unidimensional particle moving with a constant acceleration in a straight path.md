---
Date created: 2024-10-04 11:46
tags:
  - Type/Refined_Note
  - Topic/Physics
---

---

Types: _Not applicable_
Examples: _Not applicable_
Properties: _Not applicable_

Justifications: [[Unidimensional kinematics]]
Specializations: _Not applicable_
Generalization: _Not applicable_

---

A particle moving in one dimension at some constant acceleration has a position with respect to time described by $$ x(t)=x_{0} +v_{0}(t-t_{0})+\frac{a}{2}(t-t_{0})$$Here $x_{0}$ is the particles initial position, $v_{0}$ it's initial speed and $t_{0}$ the initial moment we start studying the particles movement. For the grand majority of cases, we take $t_{0}=0$

>[!quote]- Deriving the equation
>In order to derive the equation, we start with the only relevant information we really have, mainly that $$ a=\frac{dv}{dt} $$We can solve this differential equation by integrating on both side and obtain $$ \int_{t_{0}}^{t}a\; dt= \int_{t_{0}}^{t} \frac{dv}{dt}\;dt  $$This gives us $$ a(t-t_{0})= \int_{t_{0}}^{t} \frac{dv}{dt}\;dt$$ We can make the substitution $v=v$, which means that $dv=\frac{dv}{dt}dt$, meaning that we can write $$ a(t-t_{0})=v-v_{0} $$But we can simply further by remembering that $v=\frac{dx}{dt}$, and then integrate once again on both sides $$\begin{align}  \int_{t_{0}}^{t}a(t-t_{0})\;dt&=\int_{t_{0}}^{t} \frac{dx}{dt}-v_{0}\; dt \\&=-v_{0}(t-t_{0})+\int_{t_{0}}^{t} \frac{dx}{dt}\;dt  \end{align}$$We can do a similar change of variable to solve the right integral, whilst the left integral is very straight forward to solve. We obtain $$ \frac{a}{2}(t-t_{0})^{2}+v_{0}(t-t_{0})+x_{0}=x $$


