
---

mathLink: Euclidian algorithm in $\mathbb N$

---
Date created: 2023-11-24 22:24
Tags: #Type/Unfinished  #Type/Notion #Topic/Real_Analysis 

Types: %%_Objects/notions of type `object`/`notion` with additional restrictions._%% 
Examples: %%_Specific examples or counterexamples of `object`/`notion` (but not of any of its `types`)._%%
Construction: %%_Objects/notions derived from `object`/`notion`._%%
Generalization: %%_Abstractions of `object`/`notion`._%%

Properties: %%_Statements regarding `object` or necessary conditions of `notion`._%%
Sufficiencies: %%_Proofs that other objects are of type `object` or sufficient conditions of `notion`._%%
Equivalences: %%_Equivalent definitions for `object` or biconditionals between notions and `notion`._%%
Justifications: %%_Proofs of well-definition of `object`/`notion`._%%

---  

[[Natural numbers]]

> [!quote] Notion:
> Lorem ipsum dolor sit amet


Let $n$ be a natural number, and let $q$ be a positive number. Then there exist natural numbers $m$, $r$ such that $0 \leq r <q$ and $n=mq+r$ .

In other word we can "divide" a natural number $n$ by $q$ and obtain the quotient $m$ and the remainder $r$ 


#### *Proof*

We will prove this by induction on $n$ and fixing $q$ . First we study the base case $n=0$ which produces the statement $0=mq+r$ and we see that this is true for $m=0$ and $r=0$. Now we assume for our induction hypothesis that $\exists m,r :(n=mq+r \land 0 \leq r <q)$ . We need to prove that this implies the truth of $\exists m',r' :(n+1=m'q+r' \land 0 \leq r' <q)$ . We know that $n$ can be rewritten in the expression so we obtain $mq+r+1=m'q+r'$ . Now depending on the values of $r$ we have different solutions. Suppose $r+1\neq q$ , then choosing $m'=m$ and $r'=r+1$ gives us a true statement since it respects $0 \leq r' <q$ and $m'q+r'=mq+r+1=n+1$ . Suppose $r+1=q$ . Then we take $m'=m+1$ and $r'=0$ . Which implies $m'q+r'=(m+1)q +0$ and on it's turn gives us $mq+q=mq+r+1=n+1$ . This closes the induction.

**Q.E.D.**
