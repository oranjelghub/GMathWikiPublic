
---

mathLink: auto

---
Date created: 2024-03-13 16:18
Tags: #Type/Theorem  #Type/Proof #Topic/Real_Analysis 

Proved by: [[Ordering of the natural numbers]]
References: _Not applicable_
Justifications: [[Sets]], [[Cardinality of a set]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  

This important theorem justifies the existence and use of the notation $\min(X)$ where $X\subseteq \mathbb{N}$.

> [!quote] Theorem: Well ordering principle of the natural numbers
> Given any non-empty $X\subseteq \mathbb{N}$ there exists exactly one $\min(X)\in X$ such that for all $x\in X$, $\min(X)\leq x$.

>[!quote] Proof: Well ordering principle of the natural numbers
>One can easily show that this holds for any finite set through induction on the cardinality of that set. Take some arbitrary $k\in X$, we define $$ X_{k} :=\left\{ x:x \in X; x<k \right\}  $$ Which is finite since clearly $$ X_{k}\subseteq [\![0,k]\!]_{\mathbb{N}} $$ Since $X_{k}$ is finite we automatically know that $\min(X_{k})$ exists and is unique. Noticing that $$X=X_{k}\cup X\backslash X_{k}$$ We conclude that every element of $X$ is either in $X_{k}$ or $X\backslash X_{k}$ because they are disjoint, meaning that for every element $a\in X$ we have $$a\in X_{k}\implies \min(X_{k})\leq a \veebar a\in X\backslash X_{k} \implies \forall x_{k}\in X_{k}; x_{k}<a $$ Thus $\min(X_{k})$ is the minimal element of $X$, regardless of the choice of $k$ (One can easily show that picking some $j\neq k$ leads to the conclusion that $\min(X_{j})=\min(X_{k})$).
>
>**Q.E.D.**

