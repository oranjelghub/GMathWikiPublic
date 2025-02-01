---
mathLink: auto
Date created: 2024-05-01 12:27
tags:
  - Type/Theorem
  - Type/Notion
  - Type/Proof
  - Topic/Set_Theory
cssclasses:
---

---

Proved by: _Not applicable_
References: _Not applicable_
Justifications: [[Axiom of choice]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

We will be listing here alternative formulations of the axiom of choice and also include the proof that shows the statements are equivalent.

---

> [!quote]- Notion: Alternative formulation 1
> Let $X$ and $Y$ be sets, and let $P(x,y)$ be a property pertaining to objects $x\in X$ and $y\in Y$ such that for every $x\in X$ there is at least one $y$ such that $P(x,y)$ is true. Then there exists a function $f:X\to Y$ such that $P(x,f(x))$ is true for all $x\in X$.

> [!quote]- Proof: Alternative formulation 1
> We first show that choice implies this formulation. Define the set $$ Y_{x}:=\left\{ y\in Y: P(x,y)\; \text{is true} \right\}  $$ By the axiom of choice $\prod_{x\in X}Y_{x}$ is non-empty and thus there exists some sequence $(y_x)_{x\in X}$. Defining $$ f:X\to Y: x\mapsto y_{x} $$ gives us a function where $P(x,f(x))$ is true for all $x\in X$. We now show the alternative statement implies choice. Consider some indexing set $I$ such that for all $\alpha\in I$, $X_{\alpha}$ is some non-empty set. We can then consider the set $\bigcup_{\beta\in I}X_{\beta}$. We also know that for every $\alpha\in I$ there is some $z\in \bigcup_{\beta\in I}X_{\beta}$ such that $z\in X_{\alpha}$, since all the $X_{\alpha}$ are non empty and thus single choice applies. Knowing this the alternative statement applies and there exists some function $f$ $$ f:I\to \bigcup_{\beta\in I}X_{\beta} \land \forall \alpha \in I, P(\alpha, f(\alpha))\; \text{is true}$$ Where $P(\alpha, f(\alpha))$ is the statement $f(\alpha)\in X_{\alpha}$. But notice that this function $f$ satisfices all the conditions for membership in $\prod_{\rho\in I}X_{\rho}$, implying it's non emptyness and thus also the axiom of choice.
> 
> **Q.E.D.**

---

>[!quote]- Notion: Alternative formulation 2
>Let $I$ be some indexing set such that for all $\alpha\in I$ there is some non-empty set $X_{\alpha}$. Suppose also that for all $\alpha,\beta\in I$, we have $X_{\alpha}\cap X_{\beta}=\emptyset$. Then there exists some set $Y$ such that for all $\alpha\in I$, we have $\#(Y\cap X_{\alpha})=1$.

>[!quote]- Proof: Alternative formulation 2
>First we proof choice implies this. We will not give a whole explanation as it is quite trivial. Consider $f\in \prod_{\alpha\in I}X_{\alpha}$, then $f(I)$ is a set satisfying the conditions of alternative formulation 2. Now we want to prove that the formulation implies choice. Consider for every $\alpha\in I$ the set $\{ \alpha \}\times X_{\alpha}$, they are all disjoint and thus there is some set $Y$ that shares exactly one element with each set. One could then let the set induce a function $f$, which would satisfy the membership condition of $\prod_{\alpha\in I}X_{\alpha}$ and thus make it non-empty, implying choice.
>
>**Q.E.D.**

---

>[!quote]- Notion: Alternative formulation 2
>Let $A$ and $B$ be sets such that there exists a surjection $g:B\to A$, then there exists a injection $f:A\to B$.

>[!quote]- Proof: Alternative formulation 2
>We first show choice implies the formulation. Suppose we have some surjection $g:B\to A$, then the sets $g^{-1}(\{ a \})$ are all non empty and thus by the axiom of choice $\prod_{a\in A}g^{-1}(\{ a \})$ is also non-empty. This being said, pick some arbitrary $(x_{a})_{a\in A}\in \prod_{a\in A}g^{-1}(\{ a \})$ and define $f:A\to B:a\mapsto x_{a}$. Notice this is clearly an injection because otherwise it would contradict $g$ being a well defined surjection. Now we prove the formulation implies the axiom of choice. Suppose we have some arbitrary collection of non-empty arbitrary sets $\{ A_{\alpha} \}_{\alpha\in I}$ and their associated surjection $g_{\alpha}:A_{\alpha}\to \{ \alpha \}$. By the alternative formulation we know that there thus exists a injection $f_{\alpha}:\{ \alpha \}\to A_{\alpha}$. Notice that we can now define $$ x_{\alpha}:=f_{\alpha}(\alpha) $$ Notice that this sequence satisfies the necessary conditions for membership in $\prod_{\alpha\in I}X_{\alpha}$. Thus the axiom of choice is true.
>
>**Q.E.D.**

