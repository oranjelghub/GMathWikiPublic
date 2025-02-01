---
mathLink: auto
Date created: 2024-05-06 16:42
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Set_Theory
cssclasses:
---

---

Proved by: [[Zorn's lemma]], [[Alternative formulations and examples of the axiom of choice]]
References: _Not applicable_
Justifications: [[Axiom of choice]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

The proof of Zorn's lemma requires choice, so we know that one already implies the other.

> [!quote] Theorem: Zorn's lemma is logically equivalent to the axiom of choice
> The truth of Zorn's lemma implies the axiom of choice.

>[!quote] Proof: Zorn's lemma is logically equivalent to the axiom of choice
>We will do this by proving one of the equivalent statements of choice ([[Alternative formulations and examples of the axiom of choice]]). Let $I$ be a non-empty set and let $\{ X_{\alpha} \}_{\alpha\in I}$ be a family of disjoint sets. We define $$ \Omega:=\left\{  Y\subseteq \bigcup_{\alpha\in I}X_{\alpha}: \forall \alpha\in I, \left| Y\cap X_{\alpha} \right|\leq 1   \right\} $$ Consider $(\Omega, \subseteq)$, take some totally ordered subset $T\subseteq \Omega$, notice that it is bounded above by $\bigcup T$ and thus there is some maximal element $\mathcal{Y}\in \Omega$. We now claim this maximal element satisfies $$\forall \alpha\in I: \left| \mathcal{Y}\cap X_{\alpha} \right|=1 $$ Which must be true, because otherwise this would introduce a contradiction pretty quickly. Namely we know that $\left| \mathcal{Y}\cap X_{\mu } \right|=0$ for some $\mu\in I$, thus pick some $x_{\mu}\in X_{\mu}$ and notice that $\mathcal{Y}\subseteq \mathcal{Y}\cup \{ x_{\mu} \}$, a contradiction. Thus there exists some $\mathcal{Y}$ that satisfies the aforementioned property, but we know this is a logical equivalent to choice. Thus Zorn's lemma implies the axiom of choice.
>
>**Q.E.D.**

