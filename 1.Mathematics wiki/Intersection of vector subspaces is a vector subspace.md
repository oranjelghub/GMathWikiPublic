---
mathLink: auto
Date created: 2023-11-26 23:31
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Linear_Algebra
cssclasses:
---

---

Proved by: [[Vector subspace criterium]]
References: _Not applicable_
Justifications: %[[Vector spaces]]

Specializations: _Not applicable_*
Generalizations: _Not applicable_

---

> [!quote] Theorem: Intersection of vector subspaces is a vector subspace
> Let $\{ W_{\alpha} \}_{\alpha\in I}$ be a collection of vector subspace of some vector space $V$ over some field $F$. Then $\bigcap_{\alpha\in I}W_{\alpha}$ is also a vector subspace of $V$.

>[!quote] Proof: Intersection of vector subspaces is a vector subspace
>We proceed by the three criterium of a vector subspace. Notice first of all that $\bigcap_{\alpha\in I}W_{\alpha}$ is not empty because $0\in W_{\alpha}$ for all $\alpha\in I$. Now fix two vectors $w_{1},w_{2}\in \bigcap_{\alpha\in I}W_{\alpha}$ We have that for all $\alpha\in I$, $w_{1},w_{2}\in W_{\alpha}$. Since $W_{\alpha}$ is a vector subspace we know that $w_{1}+w_{2}\in W_{\alpha}$, but this is true for all the $\alpha\in I$, thus $w_{1}+w_{2}\in \bigcap_{\alpha\in I}W_{\alpha}$. We finish the proof with closure under scalar multiplication. Let $f\in F$ and $w_{3}\in \bigcap_{\alpha\in I}W_{\alpha}$, then for all $\alpha\in I$ we know that $fw_{3}\in W_{\alpha}$, in other words $fw_{3}\in \bigcap_{\alpha\in I}W_{\alpha}$. This proves that $\bigcap_{\alpha\in I}W_{\alpha}$ is a vector subspace of $V$.


