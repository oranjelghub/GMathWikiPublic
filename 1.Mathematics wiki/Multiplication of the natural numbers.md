
---

mathLink: auto

---
Date created: 2023-10-21 22:19
Tags: #Type/Notion #Topic/Number_Theory #Topic/Real_Analysis 

Types: _Not applicable_
Examples: _Not applicable_
Construction: [[Semiring of natural numbers]]
Generalization: [[Multiplication]], [[Binary operations]]

Properties: _Not applicable_
Sufficiencies: [[Natural numbers]]
Equivalences: _Not applicable_
Justifications: [[Multiplication is well defined in N]]

References: [[Properties of multiplication in N (Proof)]]

---  

We define multiplication (a [[Binary operations|binary operation]]) on the [[Natural numbers]] by the following recursion:

> [!quote] Notion: Multiplication in the natural numbers
>$$0 \times m:=0 \hspace{1cm} (1)$$ $$S(n) \times m:=(n\times m)+m \hspace{1cm} (2)$$

From this follows the properties of the multiplication in $\mathbb N$.

> [!quote] Proposition: Properties of multiplication in N
> 1. $m\times0=0$
> 2. $n \times S(m) = (n\times m)+n$
> 3. $n,m\in \mathbb{N}:n\times m=q \implies q \in \mathbb{N}$
> 4. $n\times m =m \times n$ (Commutativity of multiplication)
> 5. $n,m \in \mathbb{N}: n\times m = 0 \iff  n =0 \lor m=0$ (Absence of zero divisors)
> 6. $a,b,c \in \mathbb{N} :a(b + c) = ab + ac \land (b + c)a = ba + ca$ (Distributive law)
> 7. $a,b,c \in \mathbb{N} :(a \times b) \times c = a \times (b \times c)$ (Associativity of multiplication)
> 8. $ac=bc \land c \in \mathbb{N}_0 \implies a=b$ (Cancellation law)

---

**_Remark_**: We usually write $a\times b=ab$ for a simplified notation.