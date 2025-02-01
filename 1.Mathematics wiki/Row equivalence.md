---
mathLink: auto
Date created: 2024-09-01 12:03
tags:
  - Type/Object
  - Topic/Linear_Algebra
cssclasses:
---

---  

Types: _Not applicable_
Examples: _Not applicable_
Construction: _Not applicable_
Generalization: _Not applicable_

Properties: [[Every matrix is row equivalent to some row reduced echelon form matrix]]
Sufficiencies: _Not applicable_
Equivalences: _Not applicable_
Justifications: [[Elementary matrices]], [[Matrix multiplication]], [[Matrices]]

---

> [!quote] Definition: Row equivalence
> Two matrices $A,B\in M_{n\times m}(F)$ are said to be row equivalent if and only if $$ \{ C_{i} \}_{1\leq i\leq k}\subseteq \mathbf{E}(A): \left( \prod_{i=1}^{k}C_{k-i+1}  \right)*A=B  $$

Where $\prod$ is the matrix product and $$ \prod^{k}_{i=1}C_{i}=C_{1}*\left( \prod^{k}_{i=2}C_{i} \right)=\left( \prod^{k-1}_{i=1}C_{i} \right)*C_{k}  $$
