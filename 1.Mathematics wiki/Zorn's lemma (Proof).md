---
mathLink: auto
Date created: 2024-05-01 16:32
tags:
  - Type/Proof
  - Topic/Set_Theory
cssclasses:
---

---  

Proved by: [[Axiom of choice]]
References: _Not applicable_
Justifications: [[Sets]], [[Partially ordered set]], [[Totally ordered set]], [[Bounds, strict bounds, minimal and maximal elements of a set]]

Specializations: _Not applicable_
Generalizations: _Not applicable_

---

**WARNING: the proof is very long and painfull, good luck.**

---

> [!quote] Proof: Zorn's lemma
> We split this proof up in two big parts. We first start by proving a lemma and then proceed to use it to prove Zorn's lemma. 
> 
> We thus start by proving the following lemma: Let $X$ be a partially ordered set with ordering $\leq$, and let $x_{0}$ be some element of $X$. Then there exists a well-ordered subset $Y$ of $X$ which has no strict upper bound and has $x_{0}$ as it's minimal element. We will proceed by contradiction, so suppose this isn't the case. This would mean every well-ordered subset of $X$ containing $x_{0}$ has some upper bound in $X$. By the axiom of choice we can pick some upper bound per well-ordered set containing $x_{0}$, we thus pick some arbitrary choice function $s$ for this. We now also make a distinction between well ordered sets that contain $x_{0}$ we say a set $Y$ is good if and only if $Y$ is well ordered and $$ \forall x\in Y\backslash \{ x_{0} \},\;  s(\{ y\in Y: y<x \})=x $$ And we then proceed to define $$ \Omega:=\{ Y\subseteq X: \min Y= x_{0} \land Y\text{ is good} \} $$ $\Omega$ is already partially ordered by set inclusion but we now claim it is also totally ordered. 
> 
> We do this by noticing that given two good sets $Y,Y'$, we either have that $Y\backslash Y'$ is non-empty or $Y'\backslash Y$ is non-empty. This can be proven by first using generalized strong induction to show that $$ \forall a\in Y\cap Y',\; \{ y\in Y: y\leq a\}=\{ y\in Y': y\leq a \}=\{ y\in Y\cap Y': y\leq a \} $$ Implying that $Y\cap Y'$ is good and that $s(Y\cap Y')$ exists as well. Now suppose $Y\backslash Y'$ is non-empty, then notice that for all $a\in Y\cap Y'$ we must have that $a<\min Y\backslash Y'$ in order to avoid contradiction, thus we can rewrite $Y\cap Y'=\{ y\in Y: y<\min Y\backslash Y' \}$, and since $Y$ is good this implies $s(Y\cap Y')=\min Y\backslash Y'$. Now notice both $Y\backslash Y'$ and $Y'\backslash Y$ are disjoint, this means that if both were to be non-empty then by the previous argument we could extract a contradiction. Thus one of them must be non-empty so the argument can only be reproduced for one of the sets. Now notice that we can thus state that all the elements of $Y\backslash Y'$ are upper bounds for $Y'$ and so are the elements of $Y'\backslash Y$ for $Y$ (one of these two being true vacuously). But notice that this implies that given two arbitrary good sets $Y'$ and $Y$, that one of them is a subset of the other one, in other words we can conclude that $\Omega$ is totally ordered by set inclusion.
> 
>Now define $Y_{\infty}:=\bigcup\Omega$, notice that this set also has $x_{0}$ as it's minimal element. We claim that $Y_{\infty}$ is totally ordered. Picking two arbitrary elements $x,x'\in Y_{\infty}$ we know that they both are member of some good set $X$ and $X'$, but by the total ordening of $\Omega$ we know one of these two sets contains both $x$ and $x'$. Thus they are both member of the same good set, which is well ordered and thus we either have $x\leq x'$ or $x'\leq x$, in other words $Y_{\infty}$ is totally ordered. In addition to this we claim that $Y_{\infty}$ is well ordered. To do this pick some arbitrary non-empty $A\subseteq Y_{\infty}$ and some element $a\in A$. Since $a\in Y_{\infty}$ we know that $a\in Y$ for some good set $Y$. Now notice that $A\cap Y$ is non-empty and, by the well ordering of $Y$, has some minimal element we will call $b$. We also have that for any other good set $Y'$ that all the element of $Y'\backslash Y$ form upper bounds for $Y$, and thus $b$ is also minimal element of $A\cap Y'$ for any good set $Y$ such that $A\cap Y' \neq \emptyset$. Since every element of $A$ is member of some good set $Y'$ we must have that $b$ is the minimum of $A$ to avoid contradiction. Thus $Y_{\infty}$ is well ordered indeed. 
>
>Notice that this implies that $Y_{\infty}$ is a good set and thus by our original assumption $s(Y_{\infty})$ exists as well. Now one can pretty easily show that $Y_{\infty}\cup \{ s(Y_{\infty}) \}$ is well ordered and has $x_{0}$ as it's minimal argument. We now claim it is also good, to do this we only have to show that $s(\{ y\in Y_{\infty}\cup \{ s(Y_{\infty}) \}: y<x \})=x$ when $x\in \left( Y_{\infty}\cup \{ s(Y_{\infty}) \} \right)\backslash\{ x \}$. This is pretty obvious when $x=s(Y_{\infty})$, so suppose $x\in Y_{\infty}$. Then we know $x\in Y$ for some good set $Y$, we also notice that in this case (by the previous argument surrounding $Y\backslash Y'$ and $Y'\backslash Y$) $$ \{ y\in Y_{\infty}\cup \{ s(Y_{\infty}) \}: y<x \}= \{ y\in Y: y<x \} $$ Which implies $Y_{\infty}\cup \{ s(Y_{\infty}) \}$ is good since $Y$ is good. But now this implies that $$Y_{\infty}\cup \{ s(Y_{\infty}) \} \subseteq Y_{\infty}$$ But this is a contradiction! Since $s(Y_{\infty})$ is supposed to be a strict upper bound. Thus our very original assumption must be wrong.
>
>Which proves the our lemma: Let $X$ be a partially ordered set with ordering $\leq$, and let $x_{0}$ be some element of $X$. Then there exists a well-ordered subset $Y$ of $X$ which has no strict upper bound and has $x_{0}$ as it's minimal element.
>
>We can now proceed to the actual proof of Zorn's lemma. Suppose Zorn's lemma was false and that even with every totally ordered subset being bounded we have that there is no maximal element. Notice that this would mean that every totally ordered set with an upper bound also has a strict upper bound (otherwise the upper bound would be a maximal element). But by the previous lemma we can create a subset $Y$ of $X$ such that it is well ordered and doesn't contain a strict upper bound. In other words, a contradiction. Thus Zorn's lemma must be right in order to not contradict the big lemma we just proved. This concludes the proof. 
>
>**Q.E.D.**


