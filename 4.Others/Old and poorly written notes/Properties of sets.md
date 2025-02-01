
---

mathLink: auto

---
Date created: 2023-11-24 22:19
Tags: #Type/Unfinished  #Type/Notion #Topic/Set_Theory 

Types: %%_Objects/notions of type `object`/`notion` with additional restrictions._%% 
Examples: %%_Specific examples or counterexamples of `object`/`notion` (but not of any of its `types`)._%%
Construction: %%_Objects/notions derived from `object`/`notion`._%%
Generalization: %%_Abstractions of `object`/`notion`._%%

Properties: %%_Statements regarding `object` or necessary conditions of `notion`._%%
Sufficiencies: %%_Proofs that other objects are of type `object` or sufficient conditions of `notion`._%%
Equivalences: %%_Equivalent definitions for `object` or biconditionals between notions and `notion`._%%
Justifications: [[Properties of sets (Proof)]]

---  



> [!quote] Notion:
> Lorem ipsum dolor sit amet





#### *Properties*

-  Let $A$ be a non-empty set. Then there exists an object $x$ such that $x ∈ A$.           $$A\neq\emptyset\implies\exists x\in A\hspace{1cm}(1)$$
- The empty set is unique        $$\forall x:x\notin\emptyset \land x \notin \emptyset' \implies \emptyset=\emptyset' \hspace{1cm}(2)$$
- Singleton sets are unique: $$\forall a:\exists!\{a\} \hspace{1cm} (3)$$
- For arbitrary elements $a,b$ $$\{a,b\}=\{b,a\} \hspace{1cm}(4)$$ 
-  For arbitrary elements $a,b$ $$\{a,a\}=\{a\} \hspace{1cm} (5)$$
- Sets are partially ordered by set inclusion:
	- 1: $$A \subseteq B \land B \subseteq C \implies A \subseteq C \hspace{1cm} (6)$$
	- 2: $$A \subseteq B \land B \subseteq A \implies A=B\hspace{1cm}(7)$$
	- 3: $$A \subset B \land B \subset C \implies A\subset C\hspace{1cm}(8)$$
- Separated set is a subset: $$S=\left\{  x:x \in A\land P(x) \;\text{is true} \right\}\implies S \subseteq A \hspace{1cm}(9)$$
- The concept of separation obeys the axiom of substitution: $$A=A' \implies \{x ∈ A : P(x)\} = \{x ∈ A' : P(x)\}\hspace{1cm}(10)$$
- Consequence of axiom of regularity: $$A \notin A\hspace{1cm}(11)$$
- Consequence of axiom of regularity: $$\forall A,B:A\notin B \lor B\notin A \hspace{1cm}(12)$$



