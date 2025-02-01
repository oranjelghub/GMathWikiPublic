---
mathLink: auto
Date created: 2024-10-27 00:21
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Induction]]
References: _Not applicable_
Justifications: [[Bounded real sequences]], [[Bounded rational sequences]] 

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Finite sequences of real numbers are bounded
> Let $(a_i)^n_{i=0}$ be a finite real sequence, then $(a_i)^n_{i=0}$ is bounded.

>[!quote] Proof: Finite sequences of real numbers are bounded
>We prove this by induction on $n$. When $n = 1$ the sequence $a_1$ is clearly bounded, for if we choose $M := |a_1|$ then clearly we have $|a_i| ≤ M$ for all $1 ≤ i ≤ n$. Now suppose that we have already proved the lemma for some $n ≥ 1$; we now prove it for $n + 1$, i.e., we prove every sequence $a_1, a_2,...,a_{n+1}$ is bounded. By the induction hypothesis we know that $a_1, a_2,...,a_n$ is bounded by some $M ≥ 0$; in particular, it must be bounded by $M + |a_{n+1}|$. On the other hand, $a_{n+1}$ is also bounded by $M + |a_{n+1}|$. Thus $a_1, a_2,...,a_n, a_{n+1}$ is bounded by $M + |a_{n+1}|$, and is hence bounded. This closes the induction.
>
>**Q.E.D.**














