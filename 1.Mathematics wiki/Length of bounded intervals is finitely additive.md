---
mathLink: auto
Date created: 2024-07-17 18:09
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Real_Analysis
cssclasses:
---

---

Proved by: [[Series over finite sets (Properties)]], [[Induction]]
References: _Not applicable_
Justifications: [[Length of bounded intervals]], [[Intervals of R]]

Specializations: _Not applicable_
Generalizations: [[Lebesgue measure]], [[Alpha-length is finitely additive]]

---

> [!quote] Theorem: Length of bounded intervals is finitely additive
> Let $I$ be a bounded interval and let $P$ be a partition of cardinality $n$, then $$ \mu(I)=\sum^{}_{J\in  P}\mu (J) $$

>[!quote] Proof: Length of bounded intervals is finitely additive
>We proceed by induction on $n$. If $n=0$ then $I$ must be empty and the claim holds. Now suppose for the inductive hypothesis that $$ \mu(I)=\sum^{}_{J\in P}\mu(J) $$Where $P$ is a partition of $I$ of cardinality $n$. Now we want to prove that this implies that it also holds if we fix some partition $P$ of $I$ with cardinality $n+1$. First we may assume that $I$ is a bounded interval with endpoints $a$,$b$ and $a\neq b$, thus $I$ is either equal to $[a,b]$, $(a,b)$, $(a,b]$, $[a,b)$. We split into cases, assume first that either $I$ is equal to $(a,b]$ or $[a,b]$. Then we can fix some $K\in P$ such that $b\in K$. For some $c$ we have $a\leq c\leq b$ and $K=(c,b]$ or $K=[c,b]$ or $K=\{ b \}$ (in the case where $K$ is a singleton we fix $c:=b$). This means that $I\backslash K$ is equal to either $[a,c]$, $[a,c)$, $(a,c]$ or $(a,c)$ when $c>a$ otherwise $I\backslash K$ is empty, regardless we have $$ \mu(I)=\mu(K)+\mu(I\backslash K) $$Since $P\backslash K$ is a partition of $I\backslash K$ we have by the inductive hypothesis that $$ \mu (I\backslash K)=\sum^{}_{J\in P\backslash K}\mu(J) $$Combining the two identities with the laws of sums over finite sets we obtain $$ \mu(I)=\sum^{}_{J\in P}\mu(J) $$In the other case where $b\not\in I$ and thus $I$ is equal to either $(a,b)$ or $[a,b)$, one can pretty easily show by contradiction that there must still exist some $a\leq c\leq b$ such that $(c,b)$ or $[c,b)$ is in $P$, knowing this we may recreate the exact same argument as before and close the induction.
>
>**Q.E.D.**

