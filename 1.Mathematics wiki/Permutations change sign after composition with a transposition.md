---
mathLink: auto
Date created: 2024-09-04 15:39
tags:
  - Type/Theorem
  - Topic/Abstract_Algebra
cssclasses:
---

---

Proved by: [[Permutations change sign after composition with a elementary transposition]], [[Transpositions of N can we written as a uneven composition of elementary transpositions of N]]
References: _Not applicable_
Justifications: [[Elementary transposing permutations of N]], [[Sign of a permutation of N]]   

Specializations: [[Permutations change sign after composition with a elementary transposition]]
Generalizations: _Not applicable_

---

> [!quote] Theorem: Permutations change sign after composition with a transposition
> Let $\tau$ be a transposition and $\sigma$ a permutation of $\mathbb{N}_{\leq n}$, then $$ \text{sgn}(\tau\circ \sigma)=-\text{sgn}(\sigma) $$

>[!quote] Proof: Permutations change sign after composition with a transposition
>Since $\tau$ is a transposition we can write it as a uneven composition of elementary transpositions ${\huge{\circ}}^{2k+1}_{i=1}\tau_{e_{i}}$ with each $\tau_{e_{m}}$ elementary with respect to ${\huge{\circ}}^{m-1}_{i =1}\tau_{e_{i}}\circ\sigma$. It then follows that $$ \text{sgn}(\tau\circ \sigma)=\text{sgn}({\huge{\circ}}^{2k+1}_{i=1}\tau_{e_{i}}\circ \sigma)=(-1)^{2k+1}\text{sgn}(\sigma)=-\text{sgn}(\sigma) $$
>
>**Q.E.D.**
