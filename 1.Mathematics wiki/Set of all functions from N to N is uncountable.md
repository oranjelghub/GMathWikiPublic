---
mathLink: Set of all functions from $\mathbb N$ to $\mathbb N$ is uncountable
Date created: 2024-12-25 11:49
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Set_Theory
cssclasses:
---

---

Proved by: _Not applicable_
References: _Not applicable_
Justifications: [[Cardinality of a set]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Set of all functions from $\mathbb N$ to $\mathbb N$ is uncountable
> $$ \left| \mathbb{N}^{\mathbb{N}} \right| \neq \left| \mathbb{N} \right|  $$

>[!quote] Proof: Set of all functions from $\mathbb N$ to $\mathbb N$ is uncountable
>Let $\varphi: \mathbb{N}\to \mathbb{N}^{\mathbb{N}}$ be a function and let $f_{n}:\mathbb{N}\to \mathbb{N}$ be the function $\varphi(n)$. We define $$ g:\mathbb{N}\to \mathbb{N}: n\mapsto f_{n}(n)+1 $$Clearly $g\in \mathbb{N}^{\mathbb{N}}$. Notice now that $g\not\in \varphi(\mathbb{N})$ because if there existed $k\in \mathbb{N}$ such that $\varphi(k)=g$ then $f_{k}=g$ yet $f_{k}(k)\neq g(k)$ per construction. Thus $\varphi$ is not a surjection, hence $\mathbb{N}^{\mathbb{N}}$ is uncountable.
>
>**Q.E.D.**



