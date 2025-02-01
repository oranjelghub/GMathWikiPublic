
---

mathLink: auto

---
Date created: 2023-10-21 22:35
Tags: #Type/Proof #Topic/Number_Theory #Topic/Real_Analysis 

Proved by: [[Induction]], [[Peano axioms]], [[Addition of the natural numbers]]
References: _Not applicable_
Justifications: _Not applicable_

Specializations: _Not applicable_
Generalizations: _Not applicable_

---  

These are the proofs for the [[Multiplication of the natural numbers|properties of multiplication in N]].

> [!quote]- $m\times0=0$
> We will proceed by induction on $m$ . We first study the base case $m=0$ , in this case we have $0\times 0=0$ which is true by definition $(1)$. Then we assume that $m \times 0=0$ is true. We now have to prove that $S(m) \times 0 =0$. We will first use $(2)$ to write $(m \times 0)+0=0$ , which according to the induction hypothesis is true.
> 
> **Q.E.D.**

> [!quote]- $n \times S(m) = (n\times m)+n$
> We will prove this by induction on $n$ . We first study the base case $n=0$, which gives us $0 \times S(m) = (0\times m) + 0$ which according to $(1)$ and $(3)$ is true. Then we assume that $n \times S(m) = (n \times m) +n$ is true, we need to prove that this implies the truth of $S(n) \times S(m) = (S(n) \times m)+ S(n)$.  By $(2)$ this gives us $(n \times S(m))+S(m)= ((n \times m)+m)  + S(n)$ . By applying our inductive hypothesis we get $((n \times m)+n)+S(m)= n \times m + m + S(n)$ which implies $n \times m +n + S(m)=n \times m + m + S(n)$ which on it's turn is equal to $n \times m +S(n+m)=n \times m + S(m+n)$. This proves that both sides are equal and closes the induction.
> 
> **Q.E.D.**

> [!quote]- $n,m\in \mathbb{N}:n\times m=q \implies q \in \mathbb{N}$
> We will proceed by induction on $n$. First we analyze the base case $n=0$ which gives us $0 \times m =0$ and $0$ is a natural number so the statement is true. We now suppose that $n\times m=q$ gives us the natural number $q$, we now have to prove that multiplying by $S(n)$ still gives us a natural number. $S(n) \times m=r$ which gives us by definition $(n \times m) + m=r$ according to our hypothesis $n \times m$ was a natural number and adding two natural numbers still gives us a natural number so we show that $r$ is also a natural number which closes the induction.
> 
> **Q.E.D.**

> [!quote]- $n\times m =m \times n$ (Commutativity of multiplication)
> We will proceed by induction on $n$.  First we analyze the base case $n=0$ which gives us $0 \times m =m\times0$ and according to our definition and $(3)$ this is true. Then for our induction hypothesis we consider $n \times m= m \times n$ to be true. We now must show that this implies the truth of $S(n) \times m= m\times S(n)$. First we apply our definition and $(4)$ which obtain us $(n \times m) +m= (m \times n)+m$ and according to our hypothesis this statement is true and thus we close the induction.
> 
> **Q.E.D.**

> [!quote]- $n,m \in \mathbb{N}: n\times m = 0 \iff  n =0 \lor m=0$ (Absence of zero divisors)
> We must prove this statement in both ways. To prove it from left to right we will prove it's contrapositive which is $(n \neq 0 \lor m \neq 0) \implies nm \neq 0$ . Suppose $n$ and $m$ are positive, then there exist natural number $a$ and $b$ such that $S(a)=n$ and $S(b)=m$. Thus $nm=S(a)S(b)=(aS(b))+S(b)=((ab)+a)+S(b)=S(ab+a+b)$ which can only be positive as $0$ is not the successor of any natural number. And to prove it from right to left we suppose $n=0$ or $m=0$. Then $nm$ is always equal to zero according to our definition and $(3)$ . Thus we proved it both ways.
> 
> **Q.E.D.**

> [!quote]- $a,b,c \in \mathbb{N} :a(b + c) = ab + ac \land (b + c)a = ba + ca$ (Distributive law)
> Because of commutativity we only have to prove the left statement, which we will do by induction $c$ . First we study the base case $c=0$ which gives us the statement $a(b+0)=ab+a0$ which develops further in $ab=ab$ thanks to $(3)$. Now we suppose that $a(b+c)=ab+ac$ is true, we have to prove the truth of $a(b+S(c))=ab+aS(c)$. We develop this statement with $(4)$ $a(S(b+c))=ab+ac+a$ which is equivalent to $a(b+c)+a=ab+ac+a$ and the lest part can be further developed thanks to our induction hypotheses to give us $ab+ac+a=ab+ac+a$. This closes the induction.
> 
> **Q.E.D.**

> [!quote]- $a,b,c \in \mathbb{N} :(a \times b) \times c = a \times (b \times c)$ (Associativity of multiplication)
> We shall use induction on $c$ . First we study the base case $c=0$ which gives us the statement $(ab)0=a(b0)$ which according to the definition and $(3)$ is true. Now suppose $(ab)c=a(bc)$ is true, then we must prove that this implies the truth of $(ab)S(c)=a(bS(c))$. We develop the statement using the definition and $(4)$ $(ab)c +ab=a((bc)+b)$ using the distributive laws we get $(ab)c+ab=a(bc)+ab$ . Using our induction hypothesis shows us that the statement is true and thus we close the induction.
> 
> **Q.E.D.**

> [!quote]- $ac=bc \land c \in \mathbb{N}_0 \implies a=b$ (Cancellation law)
> By the [[Ordering of the natural numbers|trichotomy of order]], we have three cases: $a<b$,$a=b$, $a>b$ . Suppose $a<b$ then this implies $ac<ab$ which is clearly a contradiction. The same argument can be made for $a>b$ and thus the only possible option is $a=b$.




