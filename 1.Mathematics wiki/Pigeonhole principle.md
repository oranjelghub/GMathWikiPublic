
---

mathLink: auto

---
Date created: 2023-10-23 11:27
Tags: #Type/Theorem #Topic/Set_Theory 

Proved by: [[Functions]], [[Ordering of the natural numbers]], [[Cardinality of a set]], [[Union, intersection and difference of sets]]
References: _Not applicable_
Justifications: _Not applicable_   

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  

The pigeonhole principle is a theorem in set theory about [[Cardinality of a set|cardinality]] of a collection of sets that states the following:

> [!quote] Proposition: Pigeonhole principle
>  Let $A_1,...,A_n$ be finite [[Sets|sets]] such that $\#(\bigcup_{i∈\{1,...,n\}} A_i) > n$. Then there exists $i ∈ \{1,...,n\}$ such that $\#(A_i) ≥ 2$.

And it's proof goes as follows:

>[!quote]- Proof: Pigeonhole principle
> We first notice the following: $$\#(\bigcup_{i∈\{1,...,n\}} A_i) > n \implies \#(\bigcup_{i∈\{1,...,n\}} A_i) \geq S(n)$$ According to this we know that $\{1\leq i\leq S(n)\}$ must have lesser or equal [[Cardinality of a set|cardinality]] than $\bigcup_{i∈\{1,...,n\}} A_i$. This means there exists an [[Functions|injection]]. $$f:\{1\leq i\leq S(n)\} \rightarrow \bigcup_{i∈\{1,...,n\}}A_i:i\mapsto a_i$$Now suppose that indeed every set $A_i$ only contained 1 element then we have that every $i$ must map to a distinct $a_i$ which is alone in a set $A_i$. This is no problem for the first $n$ elements, but no matter how the injection is constructed, we have that $a_{S(n)}$ must be in a set $A_i$, but since every $A_i$ now already has an element, we have that at least one set must contain a second element or in other words there exists a set $A_i$ such that $\#(A_i) ≥ 2$.
> 
> **Q.E.D.**




