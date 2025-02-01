---
mathLink: auto
Date created: 2024-05-06 20:14
tags:
  - Type/Proof
  - Topic/Set_Theory
cssclasses:
---

---  

Proved by: [[Haussdorff's maximality principle]]
References: _Not applicable_
Justifications: [[Totally ordered set]], [[Zorn's lemma]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Proof: Haussdorff's maximality principle implies Zorn's lemma
> Consider $(X, \subseteq)$, by Haussdorff's maximality principle there is some maximal totally ordered subset $\mathcal{Y}$. We may also assume that $\mathcal{Y}$ is bounded above so that the condition for Zorn apply. In order to avoid a contradiction conserving the maximality of $\mathcal{Y}$ we must have that this bound, call it $M$, is a member of $\mathcal{Y}$. Implying $M=y$ for some $y\in \mathcal{Y}$. Notice that we have that $$ \nexists k\in X: y< k$$ because otherwise $\mathcal{Y}\cup \{ k \}$ would be totally ordered. Thus $y$ is a maximal element of $X$ and we know that Zorn's lemma holds.




