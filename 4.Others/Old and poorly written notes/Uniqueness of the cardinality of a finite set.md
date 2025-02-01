
---

mathLink: auto

---
Date created: 2023-12-21 14:15
Tags: #Type/Theorem #Type/Unfinished  

Proved by: %%_Statements in which `proof` depends crucially on._%%
References: %%_Notes in which the proofs of `statement` (or corollaries thereof) are delegated to._%%
Justifications: %%_Proofs of implicit assumptions of `object`/`notion` in `statement`._%%   

Specializations: %%_Reformulations/proofs of instances of `statement`._%%
Generalizations: %%_Statements and proofs of abstractions of `statement`._%%

---  



> [!quote] Theorem:
> Lorem ipsum dolor sit amet



#### *Proof of uniqueness*

We induct on $n$. First suppose that $n = 0$. Then $X$ must be empty, and so $X$ cannot have any non-zero cardinality. Now suppose that the proposition is already proven for some $n$; we now prove it for $S(n)$. Let $X$ have cardinality $S(n)$; and suppose that $X$ also has some other cardinality $m \neq S(n)$. By our lemme developed below $X$ is non-empty, and if $x$ is any element of $X$, then $X \backslash \{x\}$ has cardinality $n$ and also has cardinality $m − 1$. By induction hypothesis, this means that $n = m − 1$, which implies that $m = S(n)$, a contradiction. This closes the induction.


#### *Proof of lemma*

If $X$ is empty then it clearly cannot have the same cardinality as the non-empty set $\{i ∈ \mathbb{N} : 1 ≤ i ≤ n\}$, as there is no bijection from the empty set to a non-empty set. Now let $x$ be an element of $X$. Since $X$ has the same cardinality as $\{i ∈ \mathbb{N} : 1 ≤ i ≤ n\}$, we thus have a bijection $f$ from $X$ to $\{i ∈ \mathbb{N} : 1 ≤ i ≤ n\}$. In particular, $f(x)$ is a natural number between 1 and $n$. Now define the function $g : X \backslash \{x\} \rightarrow \{i ∈ \mathbb{N} : 1 ≤ i ≤ n − 1\}$ by the following rule: for any $y ∈ X \backslash \{x\}$, we define $g(y) := f(y)$ if $f(y) < f(x)$, and define $g(y) := f(y) − 1$ if $f(y) > f(x)$. (Note that $f(y)$ cannot equal $f(x)$ since $y \neq x$ and $f$ is a bijection.) It is easy to check that this map is also a bijection, and so $X \backslash \{x\}$ has equal cardinality with $\{i ∈ \mathbb{N} : 1 ≤ i ≤ n − 1\}$. In particular $X\backslash \{x\}$ has cardinality $n − 1$, as desired.

**Q.E.D.**



