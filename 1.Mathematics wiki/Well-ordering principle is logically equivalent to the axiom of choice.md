---
mathLink: auto
Date created: 2024-05-13 21:56
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Set_Theory
cssclasses:
---

---

Proved by: [[Well-ordering principle]]
References: _Not applicable_
Justifications: [[Well-ordering principle]], [[Axiom of choice]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Well-ordering principle is logically equivalent to the axiom of choice
> The well-ordering principle and axiom of choice are logically equivalent.

>[!quote] Proof: Well-ordering principle is logically equivalent to the axiom of choice
>We already know that we can prove the well-ordering principle using Zorn's lemma (which is an equivalent to choice), so it suffices to show that the well ordering principle is equivalent to choice. Take some set $I$ and some family of non-empty sets $\{ X_{\alpha} \}_{\alpha\in I}$, by the well ordering of principle there exists some well ordering $\leq_{\alpha}$ on $X_{\alpha}$ for every $\alpha\in I$. Now notice that the function $$ c_{I}:I\to \bigcup_{\alpha\in I} X_{\alpha}: \alpha\mapsto \min X_{\alpha} $$ is a choice function and thus the axiom of choice holds.
>
>**Q.E.D.**
