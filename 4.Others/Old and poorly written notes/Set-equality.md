


---

mathLink: auto

---
Date created: 2023-11-24 22:21
Tags: #Type/Unfinished  #Type/Notion #Topic/Set_Theory 

Types: %%_Objects/notions of type `object`/`notion` with additional restrictions._%% 
Examples: %%_Specific examples or counterexamples of `object`/`notion` (but not of any of its `types`)._%%
Construction: %%_Objects/notions derived from `object`/`notion`._%%
Generalization: %%_Abstractions of `object`/`notion`._%%

Properties: %%_Statements regarding `object` or necessary conditions of `notion`._%%
Sufficiencies: %%_Proofs that other objects are of type `object` or sufficient conditions of `notion`._%%
Equivalences: %%_Equivalent definitions for `object` or biconditionals between notions and `notion`._%%
Justifications: %%_Proofs of well-definition of `object`/`notion`._%%

---  



> [!quote] Notion:
> Lorem ipsum dolor sit amet





#### *Set equality*

We proceed to define [[Equality (binary relation)|equality]] as such: Two sets $A$ and $B$ are equal, $A = B$, if and only if every element of $A$ is an element of $B$ and vice versa. To put it another way, $A = B$ if and only if every element $x$ of $A$ belongs also to $B$, and every element $y$ of $B$ belongs also to $A$. In signs: $$(\forall a \in A:a \in B)\land(\forall b \in B:b \in A) \iff A=B$$We must also note that this equality obey the transitive, reflexive, symmetric and substitution axioms, which makes it an equality equivalent to the "$=$". 

Concerning the set equality: We can check and prove that set equality is transitive, reflexive and symmetric. But we define [[Equality (binary relation)|equality]] axiomatically, so how come we can prove this. The answer is that this set equality is defined as an axiom here. We can also assert that this implies the truth of the other properties of equality.

This approach is either not mandatory, we could also accept the following axioms:
-  Reflexive axiom, given any object $x$ we have: $$x=x$$
-  Symmetric axiom, gives any 2 objects $x$ and $y$  of the same class: $$x=y \Longleftrightarrow y=x$$
-  Transitive axiom, given any 3 objects $x$ , $y$ and $z$ of the same class: $$x=y \land y=z \implies x=z$$
-  Substitution axiom with regards to sets , given any 2 sets $x$ and $y$ and a [[Functions|function]] or operation $f$ 
	- For all sets $x$ and $y$, if $x=y$, then for all objects $z$, $z∈x$ if and only if $z∈y$.
	- For all objects $x$ and $y$, if $x=y$, then for all sets $z$, $x∈z$ if and only if $y∈z$.

Then we only need to add the axiom of extensionality:
- For all sets $x$ and $y$, if for all objects $z$, $z∈x$ if and only if $z∈y$, then $x=y$.

Otherwise we can, like Terence Tao, define the following axiom and proof all the properties of [[Equality (binary relation)|equality]]:
- For all sets $x$ and $y$, $x=y$ if and only if, for all objects $z$, $z∈x$ if and only if $z∈y$.

The main difference being that Terence Tao theory is based on first order logic without equality.
More info for further clarification here: [More info](https://en.wikipedia.org/w/index.php?title=Equality_(mathematics)&oldid=771248940#Equality_in_set_theory)

![[Equality in set theory.png]]



##### Mini proof for the equality properties in Analysis I

###### Substitution
$x \in A \land A=B \implies x\in B$ , which means that the property $\in$ preserved equality. Which means that as long as we define properties in terms of $\in$ we will have a property that preserves equality and abides the axiom of substitution.


###### Symmetry

We need to show that $A=A$ , we refer to the definition of set equality. $$(\forall a \in A:a \in A)\land(\forall a \in A:a \in A) \implies A=A$$ This is obviously true.

**Q.E.D.**


###### Reflexivity

We need to show that $A=B \iff B=A$
Both statements are true: $$(\forall a \in A:a \in B)\land(\forall b \in B:b \in A) \implies A=B$$$$(\forall b \in B:b \in A)\land(\forall a \in A:a \in B) \implies B=A$$
This implies that $A=B \iff B=A$

**Q.E.D.**

###### Transitivity

We need to show that $(A=B)\land (B=C)  \implies A=C$

$\forall a \in A : a\in B$ by definition, but we know that $B=C$ so $a\in B : a \in C$
The same can be said the other way starting from $c\in C$. Thus $A=C$ by definition.

**Q.E.D.**