---
mathLink: Set of well-orderings of a set $\mathcal W(X)$
Date created: 2024-05-13 20:55
tags:
  - Type/Object
  - Type/Notion
  - Topic/Set_Theory
cssclasses:
---

---  

Types: %%_Objects/notions of type `object`/`notion` with additional restrictions._%% 
Examples: %%_Specific examples or counterexamples of `object`/`notion` (but not of any of its `types`)._%%
Construction: [[Well-ordering principle]]
Generalization: _Not applicable_

Properties: _Not applicable_
Sufficiencies: _Not applicable_
Equivalences: _Not applicable_
Justifications: [[Well-ordered set]]

---

> [!quote] Definition: Set of well-orderings of a set
> Let $X$ be a set, we denote the set of all the pairs $(Y,\leq)$, where $Y\subseteq X$ and $\leq$ is a well ordering of $Y$, as $\mathcal{W}(X)$

Classically we order $\mathcal{W}(X)$ with the ordering relation $\preceq$ as follows

>[!quote] Definition: Ordering of $\mathcal{W}(X)$
>$$(Y,\leq)\preceq (Y',\leq') \iff (Y,\leq)=(Y',\leq')\lor \left( Y\subseteq Y' \land \exists x\in Y': Y=\{ y\in Y': y<'x \} \right) $$

From which follow the following properties

>[!quote] Properties: $(\mathcal{W}(X),\preceq)$
>1. $(\mathcal{W}(X),\preceq)$ is partially ordered
>2. $(\mathcal{W}(X),\preceq)$ contains exactly one minimal element, namely $(\emptyset, \leq_{\emptyset})$.
>3. The maximal elements of $(\mathcal{W}(X),\preceq)$ are of the form $(X,\leq)$ where $\leq$ is trivially also a well-ordering of $X$.

Notice that the uniqueness of $\leq_{\emptyset}$, follows from the fact that $(\emptyset, \leq_{\emptyset}) \preceq (\emptyset, \leq_{\emptyset}')$ and $(\emptyset, \leq_{\emptyset}')\preceq(\emptyset, \leq_{\emptyset})$.



