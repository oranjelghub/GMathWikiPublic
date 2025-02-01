
---

mathLink: Cardinality of $\mathbb{N}^{ 2}$

---
Date created: 2024-03-20 14:56
Tags: #Type/Theorem  #Type/Proof #Topic/Set_Theory 

Proved by: _Not applicable_
References: _Not applicable_
Justifications: [[Cardinality of a set]], [[Sets]], [[Cartesian product]]

Specializations: _Not applicable_
Generalizations: [[Countability of a n-fold cartesian product of countable sets]]

---  

> [!quote] Theorem: Cardinality of $\mathbb{N}^2$
> Let $\mathbb{N}$ denote the set of natural numbers, then $$ \left| \mathbb{N} \right| =\left| \mathbb{N}^{2} \right|  $$

>[!quote] Proof: Cardinality of $\mathbb{N}^{2}$
>Define $$ \begin{align} A:= \left\{ (n,m)\in \mathbb{N}^{2}: 0\leq m\leq n \right\}  \\ B:=\left\{ (n,m)\in \mathbb{N}^{2}: 0\leq n\leq m  \right\} \end{align} $$ And since $A\cup B= \mathbb{N}^{2}$, it would suffice to show the countability of both $A$ and $B$, which we will only do for $A$ as the proof is symmetric for $B$. Define the sequence $(a_n)^\infty_{n=0}$ recursively by putting $a_{0}:=0$ and $a_{n+1}:=a_{n}+n+1$. Notice that we can prove through induction that indeed $n\leq a_{n}$ and that $n<m \implies a_{n}<a_{m}$. Now consider $$ f:A\to \mathbb{N}: (n,m)\mapsto a_{n}+m $$ We now claim this function is injective, so suppose $(n,m),(n',m')\in A$ where $(n,m)\neq (n',m')$. There are three cases for $n,n'$, the case $n'=n$ means that $m\neq m'$ and it trivially follows that $f(n,m)\neq f(n',m')$. So now suppose $n'>n$ (the case $n>n'$ is proven by interchanging the two in the upcoming argument), then since $n'>n\implies n'\geq n=1$ we have that $$ f(n',m')=a_{n'}+m'>a_{n'}\geq a_{n+1}=a_{n}+n+1=a_{n}+m=f(n,m)  $$ And thus $f(n',m')\neq f(n,m)$. Meaning $f$ is injective and meaning that $f(A)$ is at most countable and so is $A$, and since assuming $A$ is finite produces immediate contradictions we must have that $A$ is countable. And thus since $\mathbb{N}^{2}=A\cup B$ and both are countable we have that $\mathbb{N}^{2}$ is countable.
>
>**Q.E.D.**



