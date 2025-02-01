---
mathLink: auto
Date created: 2024-12-09 21:46
tags:
  - Type/Object
  - Topic/Linear_Algebra
cssclasses:
---

---  

Types: _Not applicable_ 
Examples: _Not applicable_
Construction: [[Norm induced by a inner or Hermitian product space]]
Generalization: _Not applicable_

Properties: [[Cauchy-Schwarz inequality]]
Sufficiencies: _Not applicable_
Equivalences: _Not applicable_
Justifications: [[Vector spaces]]

---

**IMPORTANT:** _Some texts define a Inner product space to be both the space defined in the note [[Inner product space]] AND a Hermitian product space as described below. One should thus be careful with the term "Inner product space" as it may refer to both Hermitian and inner product spaces._

---

> [!quote] Definition: Hermitian product space
> Let $V$ be a $\mathbb{C}$-vector space. A Hermitian product $\langle \cdot,\cdot\rangle$ is a function $$ \langle \cdot , \cdot \rangle : V \times V\to \mathbb{C}: (v,w)\mapsto \langle v , w \rangle  $$ Such that the following properties are satisfied.
> 1. $$ \forall \alpha,\beta\in \mathbb{C}: \forall v,w,u\in V: \langle u , \alpha v+\beta w \rangle = \alpha\langle u , w \rangle+\beta \langle u , v \rangle   $$
> 2. $$ \forall v,w \in V: \langle v , w \rangle = \overline{\langle w , v \rangle }  $$
> 3. $$ \forall v\in V: \langle v , v \rangle \geq 0 $$
> 4. $$ \forall v\in V: \langle v , v \rangle =0 \iff v=0_{V} $$ In which case we say that $(\mathbb{C},V,+,\langle \cdot , \cdot \rangle)$ is a Hermitian product space.

Note that we request linearity in the second component. This is because of a common convention in physics, but one could very well ask this to be the case in the first component.
