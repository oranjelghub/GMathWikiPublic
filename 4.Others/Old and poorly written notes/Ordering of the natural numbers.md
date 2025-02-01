
---

mathLink: auto

---
Date created: 2023-10-21 22:43
Tags: #Type/Unfinished 

%%For Definition/Example of a notion/object%%

Types: %%_Objects/notions of type `object`/`notion` with additional restrictions._%% 
Examples: %%_Specific examples or counterexamples of `object`/`notion` (but not of any of its `types`)._%%
Construction: %%_Objects/notions derived from `object`/`notion`._%%
Generalization: %%_Abstractions of `object`/`notion`._%%

Properties: %%_Statements regarding `object` or necessary conditions of `notion`._%%
Sufficiencies: %%_Proofs that other objects are of type `object` or sufficient conditions of `notion`._%%
Equivalences: %%_Equivalent definitions for `object` or biconditionals between notions and `notion`._%%
Justifications: %%_Proofs of well-definition of `object`/`notion`._%%

%%For Proposition/Theorem of a notion/object including both`statement`/`proof` regarding `object`/`notion` it links to %%

Proved by: %%_Statements in which `proof` depends crucially on._%%
References: %%_Notes in which the proofs of `statement` (or corollaries thereof) are delegated to._%%
Justifications: %%_Proofs of implicit assumptions of `object`/`notion` in `statement`._%%   

Specializations: %%_Reformulations/proofs of instances of `statement`._%%
Generalizations: %%_Statements and proofs of abstractions of `statement`._%%

---  



> [!quote] Definition
> Lorem ipsum dolor sit amet



We will first treat ordering in terms of the [[Natural numbers]] $\mathbb{N}$

#### *Definition*

Let $n$ and $m$ be natural numbers. We say that $n$ is greater than or equal to $m$, and write $n ≥ m$ or $m ≤ n$, if and only if we have $n = m + a$ for some natural number $a$. We say that $n$ is strictly greater than $m$, and write $n>m$ or $m<n$, if and if $n ≥ m$ and $n \neq m$ . We note that (proof provided):
$$S(n)>n\hspace{1 cm}(1)$$
This is also proof the fact that there is no greatest natural number $N$ as $S(N)$ would always be greater.

#### *Properties*

For $a,b,c \in \mathbb{N}$ :

- Order is reflexive:$$a ≥ a \hspace{1 cm}(2)$$ 
- Order is transitive:$$a ≥ b\land b ≥ c \implies a ≥ c \hspace{1cm}(3)$$
- Order is anti-symmetric: $$a ≥ b \land b ≥ a \implies b=a \hspace{1cm} (4)$$
- [[Addition|addition]] preserves order:$$ a ≥ b \Longleftrightarrow a + c ≥ b + c\hspace{1cm}(5)  $$
- Succession partially preserves order: $$ a<b \Longleftrightarrow S(a)≤ b \hspace{1cm} (6)$$
- Definition strictly greater then: $$a<b \Longleftrightarrow b=a+d \land d \neq0 \hspace{1cm}(7)$$
- Trichotomy of order for the natural numbers: $$a,b\in \mathbb{N}\implies \text{exactly one of the following is true}:a<b,a=b,a>b\hspace{1cm} (8)$$
- [[Multiplication]] preserves order: $$c\in \mathbb{N}_0: a<b \implies ca<cb \hspace{1cm} (9)$$ 
##### Proofs

- (1)
	We will proceed by induction on $n$. We first study the base $n=0$ which obtains us the statement $S(0)>0$ and which is equivalent to $1>0$ which is obviously true because $1=0+1$ . We now assume for our induction hypothesis that $S(k)>k$  , which means $S(k)$ can be rewritten as a sum, we have to prove that this implies the truth of $S(S(k))>S(k)$. If this statement is true then there exists a non zero $d$ such that $S(S(k))=S(k)+d$ which is equal to $S(S(k))=S(k+d)$ . This also implies that $S(k) = k+d$, which we know is true according to our induction hypothesis and thus we close our induction.
	
	**Q.E.D.**
- (2)
	We use induction here. Lets first study the base case $a=0$ which is equivalent to the statement $0 \geq 0$ which is true because $0=0+0$ is equivalent according to properties and definition of [[Addition|addition]]. The we pose the hypothesis that $k\geq k$ is true and can we rewritten as $k=k+d$ which is true for $d=0$. We must prove that $S(k) \geq S(k)$ is true. Assuming the statement is true means that there exits a natural number $d$ such that $S(k)=S(k) +d$ . According to properties of [[Addition|addition]] this gives us $S(k)=S(k+d)$ which also implies $k=k+d$ , which according to our induction hypothesis is true and thus we close the induction.
	
	**Q.E.D.**
	
	Simple alternative:
	Since $a=a+0$ and $0$ is a natural number, $a≥a$.
- (3)
	Since $a\geq b$ there exists a $q$ such that $a=b+q$ , a similar statement can be bade about $b$ since $b \geq c$ and so $b=c+p$ for some $p$ in the natural numbers. And thus $a$ is also equal to $c+(q+p)$ which means $a \geq c$
	**Q.E.D.**
- (4)
	If $a \geq b$ then $\exists:p \in \mathbb{N}:a=b+p$ but the same can be said about be since $b \geq a$ : $\exists:q \in \mathbb{N}:b=a+q$ but we can substitute $a$ to get: $b=b+p+q$. Which implies that $p+q=0$ and which un its turn implies that $p=0 \land q=0$ . And thus $a=b$ .
	
	**Q.E.D.**
- (5)
	We first prove it from left to right. If $a \geq b$ then there exists a $d$ such that $a=b+d$ . We then add an arbitrary $c$ on each side giving us $a+c=b+d+c$ . Which clearly implies that $a+c \geq b+c$ . We now prove it from right to left. If  $a + c ≥ b + c$ then their exists a $d$ such that $a+c=b+c+d$ . We can use the cancellation law of addition to state that $a=b+d$ which in turn implies that $a\geq d$.
	
	**Q.E.D.**
- (6)
	We first prove it from left to right. We know that $a<b$ so there exists $d$ such that $b=a+d$ and that $a \neq b$ . If $d=0$ then we would have $a=b$ which is a contradiction so we know that $d \neq 0$. This means that there exists a $d'$ such that $S(d')=d$ . So we can rewrite our original statement as : $b=a+S(d')$ which after some juggling with properties gives us $b=S(a)+d'$ and which implies that $b\geq S(a)$. We now prove it from right to left. Since $S(a) \leq b$ we know there exists a $q$ such that $S(a)+q=b$ and after some juggling with properties we obtain that this implies that $a+S(q)=b$ and because $q$ exists we know it has a successor meaning that there is no way for $a=b$ and that proves that $a \leq b$ .
	
	**Q.E.D.**
- (7)
	We first prove from left to right. By definition we know that $a<b$ implies that $a\neq b$ . Now let's proceed by contradiction and assume that $d$ can be zero. Then $b=a+d$ could imply $a=b$ for $d=0$ which is a contradiction to the definitions. Now we prove it from right to left. If $b=a+d$ and $d\neq 0$ now suppose for the sake of contradiction that $a \leq b$ then $a$ may be equal to $b$, but this implies that $d$ has to be zero and thus we have a contradiction.
	
	**Q.E.D.**
- (8)
	First we note that only one of the three statements can be true, if $a>b$ then $a \neq b$ and if $b>a$ then again by definition we have $a\neq b$ . If $a<b$ and $b<a$ then this would imply $a=b$ which is clearly a contradiction. Thus as stated before, only one of the three statements may be true.  But now we also have to show that at least one statements is true. We will do this through induction on $a$. We first study the base case $a=0$ which implies that $0\leq b$ for all $b$ because if $b$ is equal to zero then we have a $a=b$ case and if $b$ is non zero then $b$ can we written as the sum $0+b$ but that also implies that $b>0$, and so our statement is correct for the base case. Now suppose the statement is true for $a$, then we have to prove it implies the truth of $S(a)$ . Since we have 3 possibilities we will discuss them all. If $a>b$ then $S(a)>b$ because $S(a)>a\; (1)$ and thus we use the transitivity of order proves this right. If $a=b$ then since $S(a)>a\;(1)$ we can substitute $a$ such that $S(a)>b$ which is just another of the 3 cases. And to finish it off suppose $a<b$ then we know that according to $(6)$that $S(a) \leq b$ which also means that either $S(a)=b$ or $S(a)<b$ which are again two of the cases we were considering and thus we close the induction and prove the statement.
	**Q.E.D.**
- (9)
	Since $a<b$ we have $b=a+d$. Multiplying by $c$ and using the distributive law we get $bc=ac+cd$. Since $d$ is positive, and $c$ is positive, $dc$ is positive, and hence $ac < bc$ as desired. 
	
	**Q.E.D.**