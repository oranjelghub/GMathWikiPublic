
---

mathLink: auto

---
Date created: 2023-11-24 22:40
Tags: #Type/Unfinished 

%%For Definition/Example of a notion/object%%

Types: %%_Objects/notions of type `object`/`notion` with additional restrictions._%% 
Examples: %%_Specific examples or counterexamples of `object`/`notion` (but not of any of its `types`)._%%
Construction: %%_Objects/notions derived from `object`/`notion`._%%
Generalization: %%_Abstractions of `object`/`notion`._%%

Properties: %%_Statements regarding `object` or necessary conditions of `notion`._%%
Sufficiencies: %%_Proofs that other objects are of type `object` or sufficient conditions of `notion`._%%
Equivalences: %%_Equivalent definitions for `object` or biconditionals between notions and `notion`._%%
Justifications: %%_Proofs of well-definition of `object`/`notion`._%%

%%For Proposition/Theorem of a notion/object including both`statement`/`proof` regarding `object`/`notion` it links to %%

Proved by: %%_Statements in which `proof` depends crucially on._%%
References: %%_Notes in which the proofs of `statement` (or corollaries thereof) are delegated to._%%
Justifications: %%_Proofs of implicit assumptions of `object`/`notion` in `statement`._%%   

Specializations: %%_Reformulations/proofs of instances of `statement`._%%
Generalizations: %%_Statements and proofs of abstractions of `statement`._%%

---  



> [!quote] Definition
> Lorem ipsum dolor sit amet




A [[Sequences|sequence]] $a_0, a_1, a_2,\ldots$ of numbers ([[Natural numbers]], integers, [[Rational numbers]], or [[Real numbers]]) is said to be in infinite descent if we have $a_n > a_{n+1}$ for all natural numbers $n$ (i.e., $a_0 > a_1 > a_2 >\ldots$)

From this flows the principle of infinite descent: it is not possible to have a sequence of natural numbers which is in infinite descent. We do notice that this does work for [[Integers]] and [[Rational numbers]].


## *Proof of principle of infinite descent*



Suppose for sake of contradiction that $a_0 > a_1 > a_2 > \ldots$ is a sequence of natural numbers which is in infinite descent. We will use induction on $k$ to show that $a_n \geq k$ for all $k \in \mathbb N$ and all $n \in \mathbb N$. (More formally, we let $P(k)$ be the statement “for each $n \in \mathbb N$, we have $a_n \geq k$”, and our goal is to prove that $P(k)$ is true for each natural number $k$.) For the base case, $k=0$, we see that $a_n \geq 0$ for all $n$, since $a_0, a_1, a_2, \ldots$ are all natural numbers. Now suppose inductively that we have $a_n \geq k$ for all $n$. We must show that $a_n \geq k+1$ for all $n$. Let n be given. Then by the inductive hypothesis, we know that $a_n \geq k$ for all $n$, so in particular for $n+1$ we have $a_{n+1} \geq k$. We also know that $a_n > a_{n+1}$ since the sequence is in infinite descent. Thus we have $a_n > k$ by transitivity of order, which means $a_n \geq k+1$. This closes the induction. Now we will obtain a contradiction. For $n=0$ and $k=a_0+1$ in particular, we must have     $a_0 \geq a_0+1$. This means $0\geq 1$, a contradiction.

**Q.E.D.**


We now give a proof for the extension beyond $\mathbb N$

The principle of infinite descent does not work if the sequence is allowed to take integer values. Indeed, define $a_n := -n$ for $n = 1, 2, 3, \ldots$. Then we have $a_{n+1} < a_n$ since $-(n+1) < -n$ (to show this more rigorously, we can start from $0 < 1$, subtract one from both sides to obtain $-1 < 0$, then add $-n$ to both sides to obtain $-n-1 < -n$). Since we have found an example of an infinite descent, it is possible to have an infinite descent.

The principle of infinite descent does not work if the sequence is allowed to take positive rational values. Two examples are $a_n := 1/n$ and $b_n := 2^{-n}$ for $n = 1,2,3,\ldots$. We’ll prove that this is an infinite descent for $a_1,a_2,a_3,\ldots$. We have $n+1 > n$, so multiplying through by $\frac{1}{n(n+1)}$ gives $1/n > 1/(n+1)$, i.e. $a_n > a_{n+1}$.

**Q.E.D.**


