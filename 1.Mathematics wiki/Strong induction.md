---
mathLink: auto
Date created: 2024-04-29 19:46
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Set_Theory
cssclasses:
---

---

Proved by: [[Induction]]
References: _Not applicable_
Justifications: [[Sets]], [[Induction]]

Specializations: _Not applicable_
Generalizations: [[Generalized strong induction]]

---

> [!quote] Theorem: Strong induction
> Let $P(n)$ be a property pertaining to the natural numbers. Suppose that $P(m_{0})$ is true for some natural number $m_{0}$ and that the following implication holds $$ \forall m: m_{0}<m<m', P(m)\text{ is true} \implies P(m') \text{is true} $$ 
> Then $P(n)$ is true for all the natural numbers.

>[!quote]- Proof: Strong induction (very old proof)
>We will prove the concept of strong induction through normal induction. Let $Q(n)$ be the property that $P(m)$ is true for all $m_0 \leq m < n$. We first study the base case $n=0$ .We first want to show $Q(0)$, which says that $P(m)$ is true for all $m_0 \leq m < 0$. This is vacuously true since there is no natural number strictly less than zero.
>
>We now pose our induction hypothesis, assume that the property $P(m)$ is true for all $m$ between $m_0 \leq m < n$ then we have to show that it implies the truth of the property $P(m)$ for all $m$ between $m_0 \leq m < S(n)$.  
>
>This gives us two possibilities, either $m_0 \leq m < n$ or $m=n$. This is because $m<S(n)\implies S(m)\leq S(n)\implies m \leq n$. We know $m=n$ or $m \neq n$; in the latter case we thus have $m<n$, so $m_0 \leq m < n$ . Thus we see that either $m_0 \leq m < n$ or $m=n$. 
>
>Since $Q(n)$ is true, we know that $P(m)$ is true for all $ $m_0 \leq m <n$. Thus in the case where $m_0 \leq m <n$, we already know that $P(m)$ is true thanks to our induction hypothesis. 
>
>To complete the proof we must now show that $P(m)$ is true in the case $m=n$, but this just comes down to proving $P(n)$ is true. Since $m_0 \leq m < S(n)$, by transitivity of order $m_0 < S(n)\implies S(m_0) \leq S(n) \implies m_0 \leq n$. Since $m_0 \leq n$ we can use the hypothesis for $P$, which says that if $Q(n)$ is true then $P(n)$ is also true and thus we see that $P(n)$ is true. This closes our induction 
>
>**Q.E.D.**

