---
mathLink: auto
Date created: 2024-07-18 21:56
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Length of bounded intervals is finitely additive]], [[Common refinement of bounded intervals]], [[Series over finite sets (Properties)]]
References: _Not applicable_
Justifications: [[Interval partition of a bounded interval]], [[Piecewise constant integral]], [[Length of bounded intervals]], [[Finer and coarser partitions of bounded intervals]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Piecewise constant integrals are well-defined
> Let $I$ be a bounded interval, let $f:I\to \mathbb{R}$ be a piecewise constant function on $I$, and let $P$ and $P'$ be two partitions such that $f$ is piecewise constant with respect to both partitions. Then $$ \sum^{}_{J\in P}c_{J} \mu(J)=\sum^{}_{J\in P'}c_{J} \mu(J) $$

>[!quote] Proof: Piecewise constant integrals are well-defined
>We first show that if $Q\preceq P$, where of course $Q$ and $P$ are partitions of $I$ such that $f$ is piecewise constant with respect to $P$, then $\sum^{}_{J\in Q}c_{J} \mu(J)=\sum^{}_{J\in P}c_{J} \mu(J)$. To show this we define for all $J\in P$ $$ \Omega_{J}:=\{ K\in Q:K\subseteq J  \} $$This set forms a partition of $J$, since it is finite, clearly $\bigcup \Omega_{J}=J$ and the element are of $\Omega_{J}$ are pairwise disjoint (follows from the fact that $Q$ is a partition of $I$). Since the length of intervals is finitely additive we have $$ \sum^{}_{J\in P}c_{J}\mu(J)=\sum^{}_{J\in P}c_{J}\sum^{}_{\alpha\in \Omega_{J}}\mu(\alpha) $$And since obviously $c_{\alpha}=c_{J}$ for all $\alpha\in \Omega_{J}$ we have $$\sum^{}_{J\in P}c_{J}\mu(J)=\sum^{}_{J\in P}\sum^{}_{\alpha\in\Omega_{J}}c_{\alpha}\mu(\alpha)$$Which one can show, through a tedious induction on the cardinality of $P$, is equal to $$ \sum^{}_{J\in P}\sum^{}_{\alpha\in\Omega_{J}}c_{\alpha}\mu(\alpha)=\sum^{}_{J\in Q}c_{J}\mu(J) $$Thus as long as $Q\preceq P$ and $f$ is piecewise constant with respect to $P$ then $$\sum^{}_{J\in Q}c_{J} \mu(J)=\sum^{}_{J\in P}c_{J} \mu(J)$$Then it follows that if $P$ and $P'$ are two arbitrary partitions of $I$ such that $f$ is piecewise constant on both that $$ \sum^{}_{J\in P}c_{J}\mu(J)=\sum^{}_{J\in P\#P'}c_{J}\mu(J)=\sum^{}_{J\in P'}c_{J}\mu(J) $$Which closes the proof.
>
>**Q.E.D.**


