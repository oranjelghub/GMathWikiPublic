---
Date created: 2024-09-27 21:24
tags:
  - Type/Refined_Note
  - Topic/Physics
---
---

Types: _Not applicable_
Examples: [[Center of mass in a semi circle with uniform density]], 
Properties: _Not applicable_

Justifications: _Not applicable_
Specializations: _Not applicable_
Generalization: [[Center of mass in a continuous 3 dimensional system with uniform density]]


---

Let $\{ p_{i} \}_{1\leq i\leq k}\subseteq \mathbb{R}^{n}$ be a collection of $k$ particles each with mass $m_{i}$. We define the center of mass to be the unique point $R\in \mathbb{R}^{n}$ that satisfies $$ \sum^{k}_{i=1}m_{i}(p_{i}-R)=\sum^{k}_{i=1}m_{i}\overrightarrow{Rp_{i}}=0 $$This means that $R$ is also equal to $$ R=\frac{ \sum^{k}_{i=1}m_{i}p_{i} }{\sum^{k}_{i=1}m_{i}} $$

>[!quote] Motivation behind the definition of center of mass
>We essentially want to define some point that represents the center of our cluster of particles. But not just the geometric center of the cluster, but rather the weighted geometric center. By weighted geometric center we mean that we take into account the individual mass of the particles and let heavier particles pull the center closer to them. One way to intuitively think about this, is to let our cluster of points define some geometric object, if you were to then put your finger exactly under/on the center of mass, the whole object would remain in equilibrium on your finger. This would intuitively require to consider the vectors between the center of mass and the points ($\overrightarrow{Rp_{i}}$), scaled by the mass $m_{i}$.


