---
mathLink: auto
Date created: 2024-05-13 21:27
tags:
  - Type/Theorem
  - Type/Proof
  - Topic/Set_Theory
cssclasses:
---

---

Proved by: [[Zorn's lemma]], [[Set of well-orderings of a set]]
References: _Not applicable_
Justifications: [[Axiom of choice]], [[Set of well-orderings of a set]]  

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

> [!quote] Theorem: Well-ordering principle
> Given a set $X$ there exists some relation $\leq$ on $X$ such that $X$ is well ordered.

This theorem also implies the axiom of choice by implying Zorn's lemma, this is done here: [[Well-ordering principle is logically equivalent to the axiom of choice]]

>[!quote] Proof: Well-ordering principle
>Take any totally ordered subset $T$ of $\mathcal{W}(X)$. We define $$\begin{align} S_{T}&:=\{ Y\in \mathcal{P}(X): (Y,\leq)\in T \text{ for some well ordering of } Y \} \\ O_{T}&:=\{ \leq : (Y,\leq)\in T \text{ for some }Y\in \mathcal{P}(X) \}  \end{align} $$ Now notice that for every $(Y,\leq)\in T$ we have that $$ (Y,\leq)\preceq (\bigcup S_{T}, \leq_{O_{T}} ) $$ Where we define $$\forall y,y'\in \bigcup S_{T}, y\leq_{O_{T}} y' \iff \exists \leq \in O_{T}: y\leq y'$$ One could check that indeed $\leq_{O_{T}}$ is a well-ordering of $\bigcup S_{T}$. This being said it also follows that $(\bigcup S_{T}, \leq_{O_{T}} )$ is a upper bound of $T$, thus by Zorn's lemma $\mathcal{W}(X)$ has some maximal element, which by the theory around $\mathcal{W}(X)$ is of the form $(X,\leq)$, where $\leq$ is a well-ordering of $X$.
>
>**Q.E.D.**


