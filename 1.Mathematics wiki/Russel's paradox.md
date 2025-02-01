
---

mathLink: auto

---
Date created: 2023-11-24 22:27
Tags: #Type/Notion #Topic/Set_Theory 

Types: _Not applicable_
Examples: _Not applicable_
Construction: _Not applicable_
Generalization: _Not applicable_

Properties: _Not applicable_
Sufficiencies: _Not applicable_
Equivalences: _Not applicable_
Justifications: [[ZF-axioms]], [[Sets]]

---  

Russel's paradox is a logical fallacy that appears when using the axiom of [[Sets|universal specification]] in set theory. The paradox goes as follows:

> [!quote] Notion: Russel's paradox
> Let $P(x)$ be the statement $P(x) \iff x \;\text{is a set} \land x \notin x$ . This property is thus true for all sets that do not contain themselves. But when we introduce sets like the set of all sets, this property is false. We also know this set exists thanks to the axiom of [[Sets|universal specification]].
Now use the axiom once again to create the following set: $\Omega:= \{x : P(x) \;\text{is true}\} = \{x : x \;\text{is a set and}\; x \notin x\}$ . This is the set of all sets that do not contain themselves. Now we ask ourselves the question, is $\Omega \in \Omega$ ? If $\Omega$ did contain itself then by definition $P(\Omega)$ would be true but $P(\Omega)$ would state that $\Omega$ is a set and that $\Omega \notin \Omega$, which is already a big paradox/contradiction. But this can also be done the other way around. Suppose $\Omega$ did not contain itself, then it satisfies the property $P$ and $P(\Omega)$ is true meaning that by definition $\Omega \in \Omega$ which is once again a paradox/contradiction.

In Terence Tao's Analysis I there is some interesting additional discussion provided:

>[!quote]- Notion: Additional discussion
>The problem with this axiom is that it essentially creates to "large" sets, we get sets that contain themselves which is a silly state of affairs that can lead to a plethora of problems. One way to intuitively solve this is by defining a hierarchy. Suppose we have primitive objects, like numbers. Then, primitive sets, which are sets containing numbers and other primitive sets. The point is that at each stage of the hierarchy we only see sets whose elements consist of objects at lower stages of the hierarchy, and so at no stage do we ever construct a set which contains itself. This can be translated formally into an axiom.
>
>"One can legitimately ask whether we really need this axiom in our set theory, as it is certainly less intuitive than our other axioms. For the purposes of doing analysis, it turns out in fact that this axiom is never needed; all the sets we consider in analysis are typically very low on the hierarchy of objects, for instance being sets of primitive objects, or sets of sets of primitive objects, or at worst sets of sets of sets of primitive objects. However it is necessary to include this axiom in order to perform more advanced set theory, and so we have included this axiom in the text (but in an optional section) for sake of completeness." Terence Tao
>
>To solve this we can add the following axiom, also called the axiom of regularity or axiom of foundation:
If $A$ is a non-empty set, then there is at least one element $x$ of $A$ which is either not a set, or is disjoint from $A$.





