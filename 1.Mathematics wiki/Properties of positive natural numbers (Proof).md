
---

mathLink: auto

---
Date created: 2023-10-21 20:42
Tags: #Type/Proof #Topic/Number_Theory 

Proved by: [[Induction]], [[Peano axioms]]
References: _Not applicable_
Justifications: [[Addition of the natural numbers]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  

These are the proofs for the properties of [[Positive natural numbers]].

> [!quote]- $a\neq 0\land a,b\in \mathbb N\implies a+b\;\text{is positive}$
> We will use induction on $b$. First we study the base case $b=0$. Then we have $a+0$ which is equal to $a$ according to $(3)$ and is also positive according to the definition of $a$. Then we pose our induction hypothesis. Let $a+b$ be positive, then it must imply that $a+S(b)$ is positive. From (4) we know that $a+S(b)$ equals $S(a+b)$, but we also know that $0$ cannot be the successor of any natural number according to the [[Peano axioms]]. Which thus implies $S(a+b)$ is positive. This closes the induction. 
> 
> **Q.E.D.**
> 

> [!quote]- $a,b\in \mathbb N\land a+b=0\iff a,b=0$
> We will prove this by contradiction. Suppose $a \neq 0 \lor b \neq 0$ . This means that either $a$ or $b$ is positive by definition and that their sum also is $(8)$.  But their sum is equal to $0$ which clearly isn't positive and thus we have obtained a contradiction.
> 
> **Q.E.D.**

> [!quote]- $a\in \mathbb N^{+}\implies \exists! b:S(b)=a$
> We will proceed by induction on $a$. We first see that the base case $a=0$ is vacuously true as 0 isn't the successor of any number. Now suppose inductively that the statement is true for $a=k$, then we have to show it is true for $a=S(k)$ . To show that we must prove that $S(b)=S(k)$ has a solution and also that it is unique. We can first see that $k=b$ is a solution to $S(b)=S(k)$. To prove the uniqueness suppose their are two natural numbers $b_1$ and $b_2$ such that $S(b_1) =S(k)=S(b_2)$ . Then we know that $S(b_1)=S(b_2)$ and since according to the [[Peano axioms]] the succesor is an injection we know this implies that $b_1=b_2$ , which clearly proves that the answer $k=b$ is unique. Thus closing the induction.
> 
> **Q.E.D.**





