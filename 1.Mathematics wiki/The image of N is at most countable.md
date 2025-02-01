
---

mathLink: The image of $\mathbb{N}$ is at most countable

---
Date created: 2024-03-14 16:13
Tags: #Type/Theorem  #Type/Proof #Topic/Real_Analysis #Topic/Set_Theory 

Proved by: [[Preservation of at most countability under sub-setting]], [[Well ordering of the natural numbers]]
References: _Not applicable_
Justifications: [[Cardinality of a set]], [[Natural numbers]]  

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  

> [!quote] Theorem: The image of $\mathbb{N}$ is at most countable
> Let $Y$ be a set and let $f:\mathbb{N}\to Y$ be some function. Then $f(\mathbb{N})$ is at most countable.

>[!quote] Proof: The image of $\mathbb{N}$ is at most countable
>Notice first that the following restriction on $f$ makes it surjective by definition $f':\mathbb{N}\to f(\mathbb{N}):n\mapsto f(n)$. We would like to restrict the domain further in order to get a bijection. Thus consider $x\in f(\mathbb{N})$, we define the set $$ A_{x}:=\{ n\in \mathbb{N}: f(n)=k \} $$ Which is never empty as $f$ is surjective on $f(\mathbb{N})$, and thus we can define $$ \mathcal{L}_{x}:=\min(A_{x}) $$ Now we know that $\{ \mathcal{L}_{x} \}_{x\in f(\mathbb{N})}$ is by definition a subset of $\mathbb{N}$ and thus at most countable. We would like to show now that the following restriction makes the function bijective $$ f'': \{ \mathcal{L}_{x} \}_{x\in f(\mathbb{N})}\to f(\mathbb{N}): \mathcal{L}_{x} \mapsto f(\mathcal{L}_{x}) $$ Notice it is injective by definition since $$\mathcal{L}_{a}\neq \mathcal{L}_{b}\implies f''(\mathcal{L}_{a})\neq f''(\mathcal{L}_{b})$$ And by definition of $\mathcal{L}_{x}$, $f''$ is still surjective and thus bijective. This means it has $f(\mathbb{N})$ has the same cardinality as $\{ \mathcal{L}_{x} \}_{x\in f(\mathbb{N})}$ and is thus also at most countable.
>
>**Q.E.D.**


