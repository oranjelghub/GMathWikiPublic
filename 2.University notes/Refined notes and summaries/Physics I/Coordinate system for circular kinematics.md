---
Date created: 2024-10-06 13:38
tags:
  - Type/Refined_Note
  - Topic/Physics
---

---

Types: _Not applicable_
Examples: _Not applicable_
Properties: [[Speed and acceleration in circular kinematics]]

Justifications: _Not applicable_
Specializations: _Not applicable_
Generalization: _Not applicable_

---

In circular kinematics we don't work with one fixed coordinate system. Instead the vectors we use to define the coordinate system are variable and depend on the vector being studied. We define $$ \hat{r}=\frac{\vec{r}}{\left|\left|r\right|\right|} $$With $\vec{r}$ being some vector in a circle with radius $r$, and $\vec{r}=r\cos(\theta)\hat{i}+r\sin(\theta)\hat{j}$. This being said we can write $$ \hat{r}=\cos(\theta)\hat{i}+\sin( \theta)\hat{j} $$This allows us to write $\vec{r}=r\hat{r}$. We also define our second variable basis vector, dependent on our original vector $\vec{r}$, mainly $$ \hat{\theta}=-\sin(\theta)\hat{i}+\cos(\theta)\hat{j} $$Notice that $\hat{r}\cdot \hat{\theta}=0$ for any vector $\vec{r}$. Defining our coordinate system this way has the interesting consequence that if we consider the angle as a function of time, that the time derivatives of our basis vectors aren't zero. We normally have $$ \frac{d\hat{i}}{dt}=\frac{d\hat{j}}{dt}=\frac{d\hat{k}}{dt}=0 $$But since our basis vectors a re variable, we have $$\begin{align} \frac{d\hat{r}}{dt}=\frac{d}{dt}\left(\cos(\theta)\hat{i}+\sin( \theta)\hat{j}  \right) = - \frac{d\theta}{dt}\sin(\theta)\hat{i}+ \frac{d\theta}{dt} \cos(\theta)\hat{j}=\hat{\theta} \frac{d\theta}{dt}\\ \frac{d\hat{\theta}}{dt}=\frac{d}{dt}\left(-\sin(\theta)\hat{i}+\cos(\theta)\hat{j}  \right) =- \frac{d\theta}{dt}\cos(\theta)\hat{i}- \frac{d\theta}{dt}\sin(\theta)\hat{j}=-\hat{r} \frac{d\theta}{dt} \end{align}$$Tow write these formulas in a more compact manner, we usually write $$ \frac{df}{dt}=\dot{f} $$





