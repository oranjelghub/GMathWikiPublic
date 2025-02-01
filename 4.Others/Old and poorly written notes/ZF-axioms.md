
---

mathLink: auto

---
Date created: 2023-11-24 22:05
Tags: #Type/Unfinished  #Type/Object #Topic/Set_Theory #COMPROMISED 

Types: %%_Objects/notions of type `object`/`notion` with additional restrictions._%% 
Examples: %%_Specific examples or counterexamples of `object`/`notion` (but not of any of its `types`)._%%
Construction: [[Sets]], [[Union of sets]], [[Intersection of sets]], [[Difference of sets]]
Generalization: 

Properties: %%_Statements regarding `object` or necessary conditions of `notion`._%%
Sufficiencies: %%_Proofs that other objects are of type `object` or sufficient conditions of `notion`._%%
Equivalences: %%_Equivalent definitions for `object` or biconditionals between notions and `notion`._%%
Justifications: %%_Proofs of well-definition of `object`/`notion`._%%

---  

**WARNING:** _This note is tagged as "COMPROMISED", meaning it is known to contain some small inaccuracy, or possibly, big mistake. It is advised not to use the note for documentation and approach reading it critically.

---

> [!quote] Definition: Axiom of extensionality
> Two sets are equal if and only if: $$\forall A\forall B[\forall x:x\in A\iff x\in B\implies A=B]$$







2. There exists a set $∅$, known as the empty set, which contains no elements, i.e., for every object $x$ we have $x \notin ∅$.
3. If $a$ is an object, then there exists a set $\{a\}$ whose only element is $a$, i.e., for every object $y$, we have $y \in \{a\}$ if and only if $y = a$; we refer to $\{a\}$ as the singleton set whose element is $a$. Furthermore, if $a$ and $b$ are objects, then there exists a set $\{a, b\}$ whose only elements are $a$ and $b$; i.e., for every object $y$, we have $y \in \{a, b\}$ if and only if $y = a$ or $y = b$; we refer to this set as the pair set formed by $a$ and $b$.
4. Pairwise union: Given any two sets $A$, $B$, there exists a set $A ∪ B$, called the union $A ∪ B$ of $A$ and $B$, whose elements consists of all the elements which belong to $A$ or $B$ or both. In other words, for any object $x$, $x \in A ∪ B \iff (x ∈ A \lor x \in B)$. 
	1. Main note: [[Union, intersection and difference of sets]]
	2. We don't usually use this axiom, we instead use the axiom of union, which is further down on the list
5. Specification or separation: Let $A$ be a set, and for each $x ∈ A$, let $P(x)$ be a property pertaining to $x$ (i.e., $P(x)$ is either a true statement or a false statement). Then there exists a set, called $\{x ∈ A : P(x) \;\text{is true}\}$ (or simply $\{x ∈ A : P(x)\}$ for short), whose elements are precisely the elements $x$ in $A$ for which $P(x)$ is true. In other words, for any object $y$, $y ∈ \{x ∈ A : P(x)\; \text{is true}\} \iff (y ∈ A \land P(y) \; \text{is true})$. 
	1. In some way this axiom is not necessary, as we can prove that the axiom of replacement (the next one) implies this axiom, meaning it is unnecessary.
6. Replacement: Let $A$ be a set. For any object $x ∈ A$, and any object $y$, suppose we have a statement $P(x, y)$ pertaining to $x$ and $y$, such that for each $x ∈ A$ there is at most one $y$ for which $P(x, y)$ is true. Then there exists a set $\{y : P(x, y) \;\text{is true for some} \;x ∈ A\}$, such that for any object $z$, $z ∈\{y : P(x, y) \;\text{is true for some} \; x ∈ A\} \iff P(x, z)\; \text{is true for some}\; x ∈ A$.
7. Infinity: There exists a set $\mathbb{N}$, whose elements are called [[Natural numbers|natural numbers]], as well as an object $0$ in $\mathbb{N}$, and an object $S(n)$ assigned to every [[Natural numbers|natural number]] $n ∈ \mathbb{N}$, such that the [[Peano axioms]] hold.
8. Universal specification (Dangerous, leads to [[Russel's paradox]], this is axiom attempts to unify axiom 5 and 6): Suppose for every object $x$ we have a property $P(x)$ pertaining to $x$ (so that for every $x$, $P(x)$ is either a true statement or a false statement). Then there exists a set $\{x : P(x)\; \text{is true}\}$ such that for every object $y$, $y ∈ \{x : P(x) \;\text{is true}\} \iff P(y) \;\text{is true}$.
	1. This asserts the existence of greater sets, like the set of all blue objects or the set of all sets.
	2. If we accept this axiom then we must also accept 9, but we also end up implying 2,3,4,5,6 and even 7 if we consider [[Natural numbers|natural numbers]] as objects. (This is a pretty straight forward this to prove, just always define your property to be the one pertaining to your axiom of choice).
9. Regularity or foundation (fixes [[Russel's paradox]]): If $A$ is a non-empty set, then there is at least one element $x$ of $A$ which is either not a set, or is disjoint from $A$.
10. Power set axiom (TETAO Analysis I): Let $X$ and $Y$ be sets. Then there exists a set, denoted $Y^X$, which consists of all the functions from $X$ to $Y$ , thus $f ∈ Y^X \iff (f \;\text{is a function with domain}\; X \;\text{and range}\; Y )$.
	1. Main note: [[Power sets]]
11. Union: Given any set $A$ consisting of only sets there is a set $B$ such that, for any element $c$, $c$ is a member of $B$ if and only if there is a set $D$ such that $c$ is a member of $D$ and $D$ is a member of $A$.
	1. Main note [[Union, intersection and difference of sets]]
	2. This axiom implies the axiom of pairwise union.

##### Proof axiom 6 implies axiom 5

Let $A$ be a set, and let $P(x)$ be a statement pertaining to objects $x\in A$. To show that the axiom of replacement implies the axiom of specification, we will construct the set $\{x \in A: P(x) \;\text{is true}\}$ using just the axiom of replacement. Let $Q(x,y)$ be the statement “$y=x$ and $P(x)$”. To use the axiom of replacement, we must verify that for each $x\in A$, the statement $Q(x,y)$ is true for at most one $y$. But for each $x\in A$, there is exactly one $y$ such that $y=x$, so it follows that for the full statement of $Q(x,y)$ there is at most one $y$ satisfying the statement. The axiom of replacement thus allows us to construct the set $\{y : y=x\text{ and }P(x)\text{ for some }x \in A\}$. We claim that this is the same set as $\{x \in A : P(x) \text{ is true}\}$. We show the inclusion both ways:

- Suppose $z \in \{x \in A : P(x) \text{ is true}\}$. Thus $z\in A$ and $P(z)$ is true. But this means that $z=x$ and $P(x)$ for some $x\in A$; specifically, there is $z\in A$ such that $z=z$ and $P(z)$. Thus $z \in \{y : y=x\text{ and }P(x)\text{ for some }x \in A\}$.
- Suppose $z \in \{y : y=x\text{ and }P(x)\text{ for some }x \in A\}$. This means that for some $x\in A$, we have $z=x$ and $P(x)$. Since $z=x$ this means we have $P(z)$ and $z\in A$ as well. Thus $z \in \{x \in A : P(x) \text{ is true}\}$.

Since both directions of the inclusion hold, this means that the two sets are equal.

**Q.E.D.**

##### Proof axiom 11 implies axiom 4

For this proof we will be using axiom 1,3 and 11. Fix two sets $A$ and $B$, since sets are objects we know that the following pair set exists $\Omega=\{A,B\}$. Now using axiom 11 we can define the following set $\bigcup \Omega$. Which is equivalent to the pairwise union $A\cup B$ but without using axiom 4. We shall proof set equality to prove this claim.
$$\bigcup\Omega=A\cup B$$
Suppose we have a $z$ in $\bigcup\Omega$ then we know that there is a set $E$ in $\Omega$ such that $z\in E$ but since $\Omega$ only consists of $A$ and $B$ we have that $z\in A$ or $z\in B$. But this implies that $z\in A\cup B$. Now we prove it starting from the other set. Suppose we have a $z$ in $A\cup B$ then we know that $z\in A \lor z\in B$. But since $\Omega=\{A,B\}$ we have that $(z\in A \lor z\in B)\land A,B \in\Omega$ meaning that $z\in\bigcup\Omega$ . Thus any set built by the axiom 4 can be built with 11, which closes the proof.

**Q.E.D.**