
---

mathLink: auto

---
Date created: 2023-11-15 12:16
Tags: #Type/Notion #Type/Unfinished 

Types: %%_Objects/notions of type `object`/`notion` with additional restrictions._%% 
Examples: %%_Specific examples or counterexamples of `object`/`notion` (but not of any of its `types`)._%%
Construction: %%_Objects/notions derived from `object`/`notion`._%%
Generalization: %%_Abstractions of `object`/`notion`._%%

Properties: %%_Statements regarding `object` or necessary conditions of `notion`._%%
Sufficiencies: %%_Proofs that other objects are of type `object` or sufficient conditions of `notion`._%%
Equivalences: %%_Equivalent definitions for `object` or biconditionals between notions and `notion`._%%
Justifications: %%_Proofs of well-definition of `object`/`notion`._%%

---  



> [!quote] Notion:
> Lorem ipsum dolor sit amet



## *Gaps in the rationals*

Despite the rationals having a denseness property they are still incomplete. There still an infinite number of "gaps" between the rationals, although this denseness property does ensure that the gaps are infinitely small. For example we have that the square root of two is not rational. ^968aa6

We can still "approach" this number infinitely by showing that for every $\varepsilon >0$, there exists a non-negative rational number $x$ such that $x^2<2<(x+\varepsilon)^2$.


#### *Proof that no rational number satisfies $x^2=2$*

Suppose by contradiction that there does exist indeed a rational number $x$ such that $x^2=2$ then we have that $\frac{p^2}{q^2}=2$. This implies that $p^2=2q^2$ which means $p$ is even since one can easily check that the square of an even number is even. Now since $p$ is even we know that it can be written as a multiple of a natural number $k$. Thus $4k^2=2q^2\implies 2k^2=q^2$ which also implies that $q$ is even and that $q=2m$ and thus we have that $x^2=\frac{p^2}{q^2}=\frac{k^2}{m^2}=2$. One can easily notice that we essentially have the second fraction has the same structure than the first one and we can thus easily show once again that $k$ and $m$ are even. But if this is the case then we must have that there exists a [[Sequences|sequence]] of even number $a$'s where the next entry is always the number such that it's double is the previous entry. More formally $(a_n)^\infty_{n=0}$ with $a_0:=p$ and $a_{n+1}:=\frac{a_n}{2}$. The same can be done for $q$ and a sequence $(b_n)^\infty_{n=0}$ . Now this means that $\frac{(a_l)^2}{(b_l)^2}=2$ for all $l\in \mathbb N$ but since one can easily verify that $a_n>a_{n+1}$ and $b_n >b_{n+1}$ the sequences are infinitely descending which is a contradiction to the [[Infinite descent|principle of infinite descent]] and thus the assumption that $(\frac{p}{q})^2=2 \land \frac{p}{q}\in \mathbb Q$ was false.

**Q.E.D.**


#### *Proof that we can get arbitrarily close to $\sqrt{2}$*

Let $ε > 0$ be rational. Suppose for sake of contradiction that there is no non-negative rational number $x$ for which $x^2 < 2 < (x + ε)^2$.This means that whenever $x$ is non-negative and $x^2 < 2$, we must also have $(x + ε)^2 < 2$ (note that $(x + ε)^2$ cannot equal to $2$, by our previous proof). Since $0^2 < 2$, we thus have $ε^2 < 2$, which then implies $(2ε)^2 < 2$, and indeed a simple induction shows that $(nε)^2 < 2$ for every natural number $n$. (Note that $nε$ is non-negative for every natural number $n$) But, by interspersing of the rationals we can find an integer $n$ such that $n > 2/ε$, which implies that $nε > 2$, which implies that $(nε)^2 > 4 > 2$, contradicting the claim that $(nε)^2 < 2$ for all natural numbers n. This contradiction gives the proof.

**Q.E.D**