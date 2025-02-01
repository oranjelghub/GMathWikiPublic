---
mathLink: auto
Date created: 2024-09-03 18:37
tags:
  - Type/Theorem
  - Topic/Abstract_Algebra
cssclasses:
---

---

Proved by: _Not applicable_
References: _Not applicable_
Justifications: [[Elementary transposing permutations of N]], [[Sign of a permutation of N]], [[Inversions of a permutation of N]]

Specializations: _Not applicable_
Generalizations: [[Permutations change sign after composition with a transposition]]

---

> [!quote] Theorem: Permutations change sign after composition with a elementary transposition
> Let $\tau_{e}$ be a elementary transposition with respect to some permutation $\sigma$ of $\mathbb{N}^{*}_{\leq n}$, then $$ \text{sgn}(\tau_{e}\circ \sigma)=-\text{sgn}(\sigma) $$

>[!quote] Proof: Permutations change sign after composition with a elementary transposition
>Since $\tau_{e}$ is a elementary transposition it must transpose some $\sigma(i)$ and some $\sigma(i)+1$. We now split in two cases. If $(\sigma^{-1}(\sigma(i)+1),i)\in \text{Inv}(\sigma)$, then clearly $(\sigma^{-1}(\sigma(i)+1),i)\notin \text{Inv}(\tau_{e}\circ\sigma)$ and we lose exactly one element (since the elementary transposition only affects this specific inversion, and does not change the membership status of any other pair in $\text{Inv}(\sigma)$). Thus in this case $$ \text{sgn}(\tau_{e}\circ \sigma)=-\text{sgn}(\sigma) $$A similar argument can be used in the case $(\sigma^{-1}(\sigma(i)+1),i)\notin \text{Inv}(\sigma)$, meaning that for all elementary transpositions $$ \text{sgn}(\tau_{e}\circ \sigma)=-\text{sgn}(\sigma) $$
>
>**Q.E.D.**
