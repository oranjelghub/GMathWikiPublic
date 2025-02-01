
---

mathLink: Countability of a $n$-fold cartesian product of countable sets

---
Date created: 2024-03-20 15:32
Tags: #Type/Theorem  #Type/Proof #Topic/Set_Theory 

Proved by: [[Induction]], [[Cardinality of N2]]
References: _Not applicable_
Justifications: %%_Proofs of implicit assumptions of `object`/`notion` in `statement`._%%   

Specializations: [[Cardinality of N2]]
Generalizations: _Not applicable_

---  

> [!quote] Theorem: Countability of a $n$-fold cartesian product of countable sets
> Let for every $i\in [\![1,n]\!]$ have some countable set $A_{i}$, then the $n$-fold cartesian product of those sets is also countable.
> $$ \left| \prod_{i=1}^n A_{i} \right|=\left| \mathbb{N} \right|  $$

>[!quote] Proof: Countability of a $n$-fold cartesian product of countable sets
>We proceed by induction on $n$. We shall also only cover the base case as the inductive step is trivial. Thus suppose $X$ and $Y$ are two countable sets. Since both are countable we know there exist some bijections $$ \begin{align} f_{X}: X\to \mathbb{N} \\ f_{Y}:Y\to \mathbb{N} \end{align} $$ From there we can construct the function $$ f_{X\times Y}:X\times Y\to \mathbb{N}^{2}: (x,y)\mapsto (f_{X}(x),f_{Y}(y)) $$ Which is obviously a bijective function, it follows that $X\times Y$ has the same cardinality as $\mathbb{N}^{2}$ which is known to be countable. Thus $X\times Y$ is countable.
>
>**QE.D.**

