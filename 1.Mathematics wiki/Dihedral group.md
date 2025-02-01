
---

mathLink: auto

---
Date created: 2023-10-25 15:41
Tags: #Type/Object #Topic/Abstract_Algebra 

Types: _Not applicable_
Examples: _Not applicable_
Construction: [[Property of dihedral group]]
Generalization: [[Groups]]

Properties: [[Order of the dihedral group]]
Sufficiencies: _Not applicable_
Equivalences: [[Generated Dihedral group]]
Justifications: [[Modular group]], [[Modular arithmetic]], [[Dihedral group is a group]], [[Permutations]]

---  

An often very important [[Groups|group]] studied for it's geometric [[Symmetry|symmetries]] is the dihedral group.

> [!quote] Definition: Dihedral group $D_{2n}$
> The group $D_{2n}$, called the dihedral group, is the group constituted of the set of all [[Symmetry|local and global symmetry]] preserving [[Permutations|permutations]] of a regular $n$-gon under the operation of [[Function composition|function composition]].

These [[Permutations]] are rotations $\sigma$ and reflections $\tau$. Describing them formally requires us to label each vertex with a number between $1$ and $n$ (obviously making sure $2$ comes after one or before). We can then describe these [[Permutations|permutations]] as follows:

>[!quote]- Definition: Rotation
>A rotation of an $n$-gon is the [[Permutations|permutation]] $\sigma$ that does the following mapping:
>$$\begin{align}\sigma: \{1\leq i\leq n\}\rightarrow\{1\leq i\leq n\}:v\mapsto \sigma(v)\end{align}$$And: $$\sigma(m)=j\implies \sigma(m+1)=(j+1)\mod{n}\lor\sigma(m+1)=(j-1)\mod{n}$$

Whilst a reflection $\tau$ is defined as:

>[!quote]- Definition: Reflection
>A reflection $\tau$ of an $n$-gon around a vertex $c$ is defined by the following mapping:
>$$\begin{align}\tau: \{1\leq i\leq n\}\rightarrow\{1\leq i\leq n\}:v\mapsto \tau(v)\\ \end{align}$$ And:
>$$\tau(c)=c \land \tau(c+k \mod{n})=c-k \mod{n} \hspace{1cm}k\in\mathbb Z$$

One would obviously need to verify this does indeed form a group ([[Dihedral group is a group]]).

We can extract the following properties from the definitions, which we will not prove with an exception for [[Property of dihedral group|5]]:

>[!quote]- Properties of the dihedral group$^{1}$
>1. $\sigma^{j},\sigma^{k}\land j\neq k\implies \sigma^j\neq\sigma^k$
>2. $|\tau|=2$
>3. $\forall \tau,\sigma,i:\tau\neq \sigma^i$
>4. $\tau\sigma^{i}\neq\tau\sigma^{j}\iff j\neq i$
>5. $\forall i:\sigma^i\tau=\tau\sigma^{-i}$

We can thus easily conclude that every element in $D_{2n}$ has a unique representation of the form $\sigma^j\tau^k$ with $1\leq j\leq n-1$ and $k=0,1$.

---

**_Remark_**$^1$: We haven't really develop a proper notation for all these properties, most of these remain very obvious so it is not really needed. 