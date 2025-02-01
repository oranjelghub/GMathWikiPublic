---
mathLink: auto
Date created: 2023-10-21 22:09
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Logic
  - Topic/Set_Theory
cssclasses:
---

---

Proved by: [[Induction]]
References: _Not applicable_
Justifications: _Not applicable_

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem:
> Let $n$ be a natural number, and let $P(m)$ be a property pertaining to the natural numbers such that $P(n_{0})$ is true and $$ m<n_{0}: P(S(m))\implies P(m) $$ 
> Then $P(m)$ is true for all $m\leq n_{0}$.
> 

>[!quote] Proof:
>We first define the property $Q(n)$ that states that if $P(n)$ is true, then $P(m)$ is true for all $m \leq n$. We shall show that $Q(n)$ is true for all $n$ by induction. We first study the base case $n=0$, this means $Q(0)$. So suppose that $P(0)$ is true. We want to show that $P(m)$ is true for all $m \leq 0$. By definition we have that $0=m+a$  and by properties of addition we have that $m=0$, but we already know that $P(0)$ is true. This closes the base case. Now suppose $Q(n)$ is true, we must show that $Q(S(n))$ is true. $Q(S(n))$ means that if $P(S(n))$ is true, then $P(m)$ is true for all $m \leq S(n)$, so suppose $P(S(n))$ is true. We know that whenever $P(S(m))$ then $P(m)$ is true, so for $m=n$ in particular this means that if $P(S(n))$ is true then $P(n)$ is true. So $P(n)$ is true because we assumed the truth of $P(S(n))$. By the induction hypothesis we thus have $P(m)$ for all $m \leq n$. Now let $m\leq S(n)$. We want to show that $P(m)$ is true. If we can show that $m\leq n$ or $m=S(n)$, then we will be done, because in either case we have already shown that $P(m)$ is true (either by induction hypothesis or assumption). In order to show this we will prove that $m \neq S(n) \implies m \leq n$. By trichotomy of order and context we know that $m<S(n)$ but by properties of order we have $S(m) \leq S(n)$ which on it's turn implies $m\leq n$. This closes induction. Now let $n$ be a natural number, and suppose $P(n)$ is true. By our work above, we know that $Q(n)$ is true. This means that $P(m)$ is true for all natural numbers $m\leq n$ as required. 
>
>**Q.E.D.**

