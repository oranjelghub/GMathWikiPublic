
Given an [[Integers|integer]] $n > 1$, called a modulus, two integers $a$ and $b$ are said to be congruent modulo $n$, if $n$ is a divisor of their difference: that is, if there is an integer $k$ such that:
$$a-b=kn$$
Congruence modulo $n$ is a congruence relation, meaning that it is an [[Equivalence relations|equivalence relation]] that is compatible with the operations of [[Addition|addition]], [[Subtraction|subtraction]], and [[Multiplication|multiplication]]. Congruence modulo $n$ is denoted:
$$a \equiv b \pmod{n}$$
The parentheses mean that $\pmod{n}$ applies to the entire equation, not just to the right-hand side (here, $b$).

This notation is not to be confused with the notation $b$ mod $n$ (without parentheses), which refers to the modulo operation, the remainder of $b$ when divided by $n$: that is, $b$ mod $n$ denotes the unique integer $r$ such that $0 ≤ r < n$ and 
$$r \equiv b\pmod{n}$$
This is being of course tightly related to the [[Integers|Euclidian algorithm of the integers]].

#### *Addition modulo $n$*

Let $S$ be the set $\{r:a \mod{n}=r\land a\in \mathbb{Z}\}$ which essentially is the set of remainders of $n$ that is $\{0,1,...,n-1\}$. We now define the [[Binary operations|binary operation]] of addition modulo $n$:
$$+_z:S^2\rightarrow S:(a,b)\mapsto r : a \mod n +_z b\mod n=a+b\mod n$$
One can easily check this operation is closed in $S$, has neutral element $0 \mod n$ or simply $0$ and every $a$ has an inverse $n-a$. The operation is also obviously associative and commutative.

This [[Binary operations|binary operation]] coupled with the set $S$ forms a [[Groups|group]] often denoted $\mathbb{Z}_n$ and is called the [[Groups|group]] of integers modulo $n$.