
---

mathLink: auto

---
Date created: 2023-11-24 22:20
Tags: #Type/Unfinished  #Type/Proof  #Topic/Set_Theory 

Proved by: %%_Statements in which `proof` depends crucially on._%%
References: %%_Notes in which the proofs of `statement` (or corollaries thereof) are delegated to._%%
Justifications: %%_Proofs of implicit assumptions of `object`/`notion` in `statement`._%%   

Specializations: %%_Reformulations/proofs of instances of `statement`._%%
Generalizations: %%_Statements and proofs of abstractions of `statement`._%%

---  



> [!quote] Proof:
> Lorem ipsum dolor sit amet




#### *Diverse random proofs and demonstrations*

- (1)
	We prove by contradiction. Suppose there does not exist any object $x$ such that $x ∈ A$. Then for all objects $x$, we have $x \notin A$. Also, by Axiom 2 we have $x \notin ∅$. Thus $x ∈ A \iff x ∈ ∅$ (both statements are equally false), and so $A = ∅$ , a contradiction.
	
	**Q.E.D.**
	In this proof the fact that all $x$ are not in $A$ is implies that $A$ is the empty set as that's literally the definition of the empty set.
- (2)
	By contradiction suppose there were 2 empty sets $\emptyset$ , $\emptyset'$. $\forall x:(x\notin \emptyset \land x\notin \emptyset')$. But by the contrapositive definition of set equality this means that $\emptyset = \emptyset'$.
	
	**Q.E.D.**
- (3)
	By the definition of the singleton set we know that $\forall y :y\in \{a\} \iff y=a$ . Assume that an arbitrary element $b$ had more than a unique singleton set. Applying the definition we would get , $\forall y :y\in \{b\} \iff y=b$ and $\forall y :y\in \{b'\} \iff y=b'$. But this means that for all $y$ , $y$ is in both sets which on it's turn implies that $b=b'$. Meaning that the singleton set of an element is effectively unique.
	
	**Q.E.D.**
- (4)
	We can prove both sets are equal by the definition of set equality. $\forall x\in \{a,b\}:x\in \{b,a\}$ and $\forall y\in \{b,a\}:y\in \{a,b\}$. And thus $\{a,b\}=\{b,a\}$.
	
	**Q.E.D.**
- (5)
	We can prove both sets are equal by the definition of set equality. $\forall x\in \{a,a\}:x\in \{a\}$ and $\forall y\in \{a\}:y\in \{a,a\}$. And thus $\{a,a\}=\{a\}$.
	
	**Q.E.D.**
- (6)
	Suppose that $A ⊆ B$ and $B ⊆ C$. To prove that $A ⊆ C$, we have to prove that every element of $A$ is an element of $C$. So, let us pick an arbitrary element $x$ of $A$. Then, since $A ⊆ B$, $x$ must then be an element of $B$. But then since $B ⊆ C$, $x$ is an element of $C$. Thus every element of $A$ is indeed an element of $C$, as claimed.
	
	**Q.E.D.**
- (7)
	We know that (definition subset) every element of $A$ is also in $B$ and we know that every element of $B$ is also in $A$. But this is just the definition for set equality and thus $A=B$
	
	**Q.E.D.**
- (8)
	Suppose that $A \subset B$ and $B \subset C$. To prove that $A \subset C$, we have to prove that every element of $A$ is an element of $C$. So, let us pick an arbitrary element $x$ of $A$. Then, since $A \subset B$, $x$ must then be an element of $B$ and we also know that there is still an element $b$ in $B$ that isn't in $A$. But then since $B \subset C$, $x$ is an element of $C$ just as $b$ is also an element of $C$. Thus every element of $A$ is indeed an element of $C$ and $A\neq C$, as claimed.
	
	**Q.E.D.**
- (9)
	By definition of $S$ we have that every $s$ in $S$ is also in $A$ and $P(s)$ is true. But $s$ being in $S$ implying that $s$ is also in $A$ is just the definition of a subset. Thus $S\subseteq A$.
	
	**Q.E.D.**
- (10)
	By expanding our definition of set equality we know that for any arbitrary $a$ in $A$ there must be a $a'$ in $A'$ such that $a=a'$ otherwise set equality wouldn't hold. By the axiom of substitution we have $a=a'\implies P(a)=P(a')$ and this implies that every element in $a$ that preserves the truth of the property has an equivalent element in $a'$ which also preserves the truth of the property meaning that the two sets under the property are equal and that separation obeys the axiom of substitution
	
	**Q.E.D.**
	I don't like this proof, pretty sure there is a fallacy somewhere.
- (11)
	For an arbitrary set $A$ we define the set $\{A\}$ thanks to the singleton axiom. We also know thanks to the axiom of regularity that there must be at least a non-set element or disjoint set in $\{A\}$. In this case we don't have a non-set element but we have 1 set, that by axiom must be disjoint so we have $A\cap \{A\}=\emptyset$. Now suppose $A\in A$ , then $A \in A\cap \{A\}$ , which contradicts the axiom.
	
	**Q.E.D.**
- (12)
	Consider the set $\{A,B\}$ which exist according to the pair axiom. Once again we apply the axiom of regularity just like in $(11)$ to see that either $A$ or $B$ must be a disjoint set from $\{A,B\}$. Suppose $A$ is disjoint, then we know that $B\notin A\cap \{A,B\}$ but we also know that $B\in\{A,B\}$ and thus it must follow that $B\notin A$. The same reasoning can be applied if $B$ is disjoint.
	
	**Q.E.D.**


