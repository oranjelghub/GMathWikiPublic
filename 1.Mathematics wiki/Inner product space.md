---
mathLink: auto
Date created: 2024-12-09 18:47
tags:
  - Type/Object
  - Topic/Linear_Algebra
cssclasses:
---

---  

Types: _Not applicable_
Examples: [[Standard inner product in Rn]], [[Standard matrix inner product]]
Construction: [[Norm induced by a inner or Hermitian product space]]
Generalization: _Not applicable_

Properties: [[Cauchy-Schwarz inequality]]
Sufficiencies: _Not applicable_
Equivalences: _Not applicable_
Justifications: [[Vector spaces]]

---

**IMPORTANT:** _Some texts define a Inner product space to be both the space defined in this note AND a Hermitian product space as described in [[Hermitian product space]]. One should thus be careful with the term "Inner product space" as it may refer to both Hermitian and inner product spaces._

---

> [!quote] Definition: Inner product space
> Let $V$ be a $\mathbb{R}$-vector space. A inner product $\langle \cdot,\cdot\rangle$ is a function $$ \langle \cdot , \cdot \rangle : V \times V\to \mathbb{R}: (v,w)\mapsto \langle v , w \rangle  $$ Such that the following properties are satisfied.
> 1. $$ \forall \alpha,\beta\in \mathbb{R}: \forall v,w,u\in V: \langle \alpha v+\beta w , u \rangle = \alpha \langle v , u \rangle +\beta \langle w , u \rangle   $$
> 2. $$ \forall v,w\in V: \langle v , w \rangle =\langle w , v \rangle  $$
> 3. $$ \forall v,v \in V : \langle v , v \rangle \geq 0$$
> 4. $$ \forall v \in V: \langle v , v \rangle =0 \iff v=0_{V} $$ In which case we say that $(\mathbb{R},V,+,\langle \cdot , \cdot \rangle)$ is a inner product space.

