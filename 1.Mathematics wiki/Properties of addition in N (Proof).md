
---

mathLink: auto

---
Date created: 2023-10-21 00:50
Tags: #Type/Proof #Topic/Number_Theory 

Proved by: [[Addition of the natural numbers]], [[Induction]], [[Peano axioms]]
References: _Not applicable_
Justifications: _Not applicable_ 

Specializations: _Not applicable_ 
Generalizations: _Not applicable_ 

---  

These are the proofs for the [[Addition of the natural numbers|properties of addition in N]]. 

> [!quote]- $n+0=n$
> We will use induction: The base case $n=0$ holds as according to $(1)$: $0+0=0$ . Now suppose inductively that $n+0=n$ , we now wish to show that $S(n) +0=S(n)$ . To do this we use $(2)$ and we show that $S(n) +0=S(n+0)$, which according to our induction hypothesis is equal to $S(n)$. Which closes the induction.
> 
>**Q.E.D.**

> [!quote]- $n+S(m)=S(n+m)$
> We will use induction. We first consider the base case $n=0$. By definition of addition and the previous property we derived wet get: $S(m)=S(m)$. Now for our induction hypothesis we state that $n+S(m)$ does equal $S(n+m)$ . We now wish to show that $S(n)+S(m)=S(S(n)+m)$ . By $(2)$ the left hand side is equal to $S(n+S(m))$ . Which according to our induction hypothesis is equal to $S(S(n+m))$.But we also know that our right hand side is equal to $S(S(n+m))$ according to $(2)$. Now both sides are equal and our induction is closes. 
> 
>**Q.E.D.**

> [!quote]- $n+m=m+n$ (Commutativity)
> Proof: We shall use induction (keeping $m$ fixed). We first study the base case $n=0$. In this case we get $0+m=m+0$ but according to (1) and the first property, this is just equivalent to $m=m$ . Now we state our induction hypothesis. Let's suppose $n+m=m+n$. Then we have to prove that $S(n)+m=m+S(n)$ . According to our definition of addition and $(4)$ , this is equivalent to $S(n+m)=S(m+n)$ . But according to our induction hypothesis $n+m=m+n$ so $S(m+n)=S(m+n)$. And thus we close the induction.
>  
>**Q.E.D.**

> [!quote]- $(a+b)+c=a+(b+c)$ (Associativity)
> Proof: We shall use induction (keeping $c$ fixed). We first study the base case of $c=0$. That leads us to $(a+b)+0 =a+(b+0)$ and according to $(3)$ and our definition of addition that statement is equivalent to $(a+b)=a+(b)$. Now we impose an induction hypothesis: $(a+b)+c=a+(b+c)$. Then we have to prove that: $(a+b)+S(c)=a+(b+S(c))$ . From $(4)$ follows that $S((a+b)+c)=a+S(b+c)$ and applying $(4)$ again gives us $S((a+b)+c)=S(a+(b+c))$ . And according to our induction hypothesis $S(a+(b+c))=S(a+(b+c))$ . The induction is thus closed.
>  
>**Q.E.D.**

> [!quote]- $a+b=a+c\implies b=a$ (Cancelation law)
> Proof: We prove this by induction on $a$. First consider the base case $a = 0$. Then we have $0 + b = 0+ c$, which by definition of addition implies that $b = c$ as desired. Now suppose inductively that we have the cancellation law for $a$ (so that $a + b = a + c$ implies $b = c$); we now have to prove the cancellation law for $S(a)$. In other words, we assume that $S(a)+ b = S(a) + c$ and need to show that $b = c$. By the definition of addition, $S(a) + b = S(a + b)$ and $S(a) + c = S(a + c)$ and so we have $S(a + b) = S(a + c)$. By [[Peano axioms]], we have $a + b = a + c$. Since we already have the cancellation law for $a$, we thus have $b = c$ as desired. This closes the induction.
>  
>**Q.E.D.**

---
**_Remark_**: _Note that the proofs are a bit outdated and thus have some wrong referencing, $(1)$ and $(2)$ refer to the two definition conditions of addition in [[Addition of the natural numbers]]._
