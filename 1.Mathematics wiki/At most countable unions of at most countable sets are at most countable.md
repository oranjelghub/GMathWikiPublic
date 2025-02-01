

---

mathLink: auto

---
Date created: 2024-03-19 17:35
Tags: #Type/Theorem  #Type/Proof #Topic/Set_Theory 

Proved by: [[Unions of at most countable sets are at most countable]]
References: _Not applicable_
Justifications: [[Axiom of choice]], [[Sets]], [[Cardinality of a set]], [[Well ordering of the natural numbers]]

Specializations: [[Unions of at most countable sets are at most countable]]
Generalizations: _Not applicable_

---  

> [!quote] Theorem: At most countable unions of at most countable sets are at most countable
> Let $I$ be a at most countable set, and let for every $\alpha\in I$ have some at most countable set $A_{\alpha}$, then the countable union of all the $A_{\alpha}$ is also countable. $$ \left| \bigcup_{\alpha\in I}A_{\alpha} \right| =\left| \mathbb{N} \right|  $$

>[!quote] Proof: At most countable unions of at most countable sets are at most countable 
>Assuming one has proven that the union of two at most countable sets is at most countable, one can extend it to any finite union of at most countable sets by induction. Thus assume that $I$ is countable. Pick some arbitrary bijection $g:\mathbb{N}\to I$ to rewrite $$ \bigcup_{\alpha\in I}A_{\alpha}=\bigcup_{n\in \mathbb{N}}A_{g(n)} $$ For every $\alpha\in I$ we define $$ \mathcal{F}_{g(n)}:=\left\{ f_{g(n)}: f_{g(n)}\;\text{is a injection from}\;A_{g(n)}\to \mathbb{N} \right\}  $$ By the axiom of choice we can pick some $$ (f_{g(n)})_{n\in \mathbb{N}}\in \prod_{n\in \mathbb{N}}\mathcal{F}_{g(n)} $$ Now also define the the number $$\forall a\in \bigcup_{n\in \mathbb{N}}A_{g(n)}, \;\mathcal{M}(a):=\min\left\{ n: a\in A_{g(n)} \right\}  $$ Which is obviously well defined for all $a\in \bigcup_{n\in \mathbb{N}}A_{g(n)}$. Now considering the function $$ \varphi: \bigcup_{n\in \mathbb{N}}A_{g(n)}\to \mathbb{N}^2: a\mapsto (\mathcal{M}(a),f_{g(\mathcal{M}(a))}(a))$$ And it follows that $\varphi$ is a injection to $\mathbb{N}^2$ meaning that $\bigcup_{n\in \mathbb{N}}A_{g(n)}$ is at most countable.
>
>**Q.E.D.**



