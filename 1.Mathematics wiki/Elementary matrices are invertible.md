---
mathLink: auto
Date created: 2024-09-06 22:34
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Linear_Algebra
cssclasses:
---

---

Proved by: _Not applicable_
References: _Not applicable_
Justifications: [[Elementary matrices]], [[Left and right inverse of a matrix]]   

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Elementary matrices are invertible
> Let $A\in M_{n\times m}(F)$ and $E\in \mathbf{E}(A)$, then $E$ is invertible

>[!quote] Proof: Elementary matrices are invertible
>Since $E\in \mathbf{E}(A)$ we know that $E$ is equal to some matrix $C_{ij}$, $M_{i}(\lambda),S_{ij}(\lambda)$. We split into cases, suppose $E=C_{ij}$ for some row $i$ and $j$. Then notice that $C_{ij}*C_{ij}=\mathbb{I}_{n}$ which means $E$ is invertible. If $E=M_{i}(\lambda)$ for some row $i$ and scalar $\lambda\in F$, then $M_{i}(\lambda)*M_{i}\left( \frac{1}{\lambda} \right)=\mathbb{I}_{n}$ and $E$ is invertible. If $E=S_{ij}(\lambda)$ for some row $i$ and $j$ and some scalar $\lambda\in F$ then $S_{ij}(\lambda)*S_{ij}(-\lambda)=\mathbb{I}_{n}$ and once again $E$ is invertible. This closes all the cases.
>
>**Q.E.D.**



