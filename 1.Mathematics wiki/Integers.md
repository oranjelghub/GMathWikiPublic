The set of integers, denoted $\mathbb{Z}$, is informally defined as follows:
$$\mathbb{Z}:=\{...,-2,-1,0,1,2,...\}$$
More formally the integers can be constructed from scratch, flowing out of the [[Natural numbers]].

## *Constructing the integers*

In order to construct the integers we will define a [[Scaffolding]] relation that is an [[Equivalence relations|equivalence relation]]. Thus we have the following definition for integers: An integer is an ordered pair in $\mathbb{N}^2$, written as $a--\;b$, on which we declare the following [[Equivalence relations|equivalence relation]]: $(a,b)\sim(c,d)\iff a+d=c+b$ and where $a--\; b:=\{(c,d)\in \mathbb{N}^2:(a,b)\sim (c,d)\}$. One would now have to verify we do indeed have an [[Equivalence relations|equivalence]] relation but this is a very straight forward thing.

Before we can prove substitution though we obviously need to define some [[Operations|operations]] first, or extend the ones from the [[Natural numbers|natural numbers]]. We thus define:
$$\begin{align}(a--\;b)+(c--\;d)&:=(a+c)--\;(b+d)\\(a--\;b)\times(c--\;d)&:=(ac+bd)--\;(ad+bc)\end{align}$$
One could thus now prove that those operations are well defined and that the [[Relations|relation]] also obeys substitution.

We also notice an obvious [[Group isomorphism]] between the [[Natural numbers|natural numbers]] and the integers.
$$n\equiv n--\;0$$
From this flows the notion of negation of the [[Natural numbers|natural numbers]] and the integers. If $(a--\;b)$ is an integer then we define it's negation $-(a--\;b)$ to be the integer $(b --\;a)$. In particular if $n$ is a positive natural number we have that $n=n--\;0$ and thus $-n=(0--\;n)$.  We can once again check that this definition is well defined.

With the notion of negation defined we can introduce the trichotomy of the integers.

Let $x$ be an integer, then exactly one of the following statements is true: $x$ is zero, $x$ is a positive [[Natural numbers|natural number]] or $x$ is the negation of a positive [[Natural numbers|natural number]] $n$. 

We thus also call the negation of a positive natural number a negative integer.

We can now finish of by defining [[Subtraction|subtraction]] in order to get rid of our [[Scaffolding|scaffolding]].
$$x-y:=x+(-y)$$
And from this flows:
$$a-b=a+(-b)=(a--\;0)+(0--\; b)=a--\;b$$
And thus our [[Scaffolding|scaffolding]] can be discarded and we are left with our classic well known integers.
#### *Proof of the trichotomy*

First we show that at least one of the three statements is true. By definition we have $x=a--\;b$ where we also have three different cases: $a>b$, $a=b$ and $a<b$. If $a>b$ then $a=b+c$ for some positive $c$ but that means that $a --\; b= c --\;0 =c$ and thus $x$ is a positive natural number. If $a=b$ then $a--\;b=a--\;a=0--\;0=0$ which means $x$ is zero. And in the case of $a<b$ then $b>a$, so that $b--\;a=n$ by the previous reasoning and thus $a --\; b= -n$ because negation is well defined. This gives us the case of $x$ is the negation of a positive natural number. Now we prove that only one can be true at most. First we note that per definition the case $x=0$ always implies the falsehood of $x$ being a positive natural number. Now suppose $x=0$ and $x$ is the negation of a natural number, then :$0=-n \implies (0--\;0)=(0--\;n)\implies 0+n=0+0\implies n=0$, a contradiction. Suppose $x$ was a positive natural number and a negation of one at the same time then $n=-m\implies (n--\;0)=(0--\;m)\implies n+m=0+0$ which contradicts a property of the natural numbers.

**Q.E.D.**



## *Properties of $\mathbb{Z}$*

- The integers form a [[Rings|commutative ring]] under addition and multiplication.
	- $\mathbb{Z}$ is an [[Groups|abelian group]] under [[Addition|addition]], meaning that: $(a + b) + c = a + (b + c)$ for all $a, b, c$ in $\mathbb{Z}$ (that is, $+$ is associative).
		- $a + b = b + a$ for all $a, b$ in $\mathbb{Z}$ (that is, $+$ is commutative).
		- There is an element $0$ in $\mathbb{Z}$ such that $a + 0 = a$ for all $a$ in $\mathbb{Z}$ (that is, $0$ is the additive identity).
		- For each $a$ in $\mathbb{Z}$ there exists $−a$ in $\mathbb{Z}$ such that $a + (−a) = 0$ (that is, $−a$ is the additive inverse of $a$).
	- $\mathbb{Z}$ is a [[Monoids|monoid]] under [[Multiplication|multiplication]], meaning that:
		- $(a · b) · c = a · (b · c)$ for all $a, b, c$ in $\mathbb{Z}$ (that is, $⋅$ is associative).
		- There is an element $1$ in $\mathbb{Z}$ such that $a · 1 = a$ and $1 · a = a$ for all $a$ in $\mathbb{Z}$ (that is, $1$ is the multiplicative identity).
	- Multiplication is distributive with respect to addition, meaning that:
		- $a · (b + c) = (a · b) + (a · c)$ for all $a, b, c$ in $\mathbb{Z}$ (left distributivity).
		- $(b + c) · a = (b · a) + (c · a)$ for all $a, b, c$ in $\mathbb{Z}$ (right distributivity).
	- Multiplication is also commutative, making it a commutative ring.
	- One would in theory have to check all these are true, but we won't do that.
- Well ordering principle: Every nonempty set of positive integers contains a smallest member. This was already a developed notion in the [[Natural numbers]]. This statement can either be assumed axiomatically or proved through the Peano axioms and induction. It's place in the grander math theory thus depends on the setting.
- Euclidian algorithm: Let $a$ and $b$ be integers with $b\geq0$. Then there exist unique integers $q$ and $r$ with the property that $a= bq + r$, where $0 \leq r < b$.


#completed 
