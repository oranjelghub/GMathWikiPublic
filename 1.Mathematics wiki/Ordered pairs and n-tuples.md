
If $x$ and $y$ are any objects (possibly equal), we define the ordered pair $(x, y)$ to be a object, consisting of $x$ as its first component and $y$ as its second component. Two ordered pairs $(x, y)$ and $(x' , y' )$ are considered equal if and only if both their components match.
$$(x, y)=(x' , y' ) \iff (x = x' \land y = y' )$$
This definition respect the usual axioms of equality.
	Frist of all we have reflexivity. We know that $(x_i)_{1\leq i \leq n}=(x_i)_{1\leq i \leq n}$ since for every $i$ we have that $x_i$=$x_i$. Then we have symmetry. Suppose $(x_i)_{1\leq i \leq n}=(y_i)_{1\leq i \leq n}$ , then we know that for every $i$ $x_i=y_i$ but since those are normal object we have that $y_i=x_i$ meaning that $(y_i)_{1\leq i \leq n}=(x_i)_{1\leq i \leq n}$. And to end of we have transitivity. Suppose $(x_i)_{1\leq i \leq n}=(y_i)_{1\leq i \leq n}$ and $(y_i)_{1\leq i \leq n}=(z_i)_{1\leq i \leq n}$ then we have that for each $i$ $x_i=y_i=z_i$ meaning that $x_i=z_i$ for all $i$ and that $(x_i)_{1\leq i \leq n}=(z_i)_{1\leq i \leq n}$.
	**Q.E.D.**

Strictly speaking, this definition is partly an axiom, because we have simply postulated that given any two objects $x$ and $y$, that an object of the form $(x, y)$ exists. However, it is possible to define an ordered pair using axioms of [[Sets|set theory]] in such a way that we do not need any further postulates. Namely by stating that for a set $X$ and $Y$ we have that:
$$(x,y):=\{\{x\},\{x,y\}\}$$
We can extend this notion from ordered pairs to $n$-tuples: Let $n$ be a natural number. An ordered $n$-tuple $(x_i)_{1≤i≤n}$ (also denoted $(x_1,...,x_n)$) is a collection of objects $x_i$, one for every natural number $i$ between $1$ and $n$; we refer to $x_i$ as the $i$'th component of the ordered $n$-tuple. Two ordered $n$-tuples $(x_i)_{1≤i≤n}$ and $(y_i)_{1≤i≤n}$ are said to be equal if and only if $x_i = y_i$ for all $1 ≤ i ≤ n$.

We can prove their existence by the following definition:
$$(x_i)_{1\leq i \leq n}:=(x_1,...,x_n):=(x_1,(x_2,(...,(x_{n-1},x_n)]$$
Here the square brackets denoted a big succession of normal brackets.
One can easily check this definition of $n$ pairs as nested pairs still abides the equality property from the top of the note. Thus this definition is valid and justifies the existence of $n$ pairs.


## *Their relation with functions*

An ordered $n$-tuple $x_1,...,x_n$ of objects is also called an ordered sequence of $n$ elements, or a finite sequence for short.
Thus the notion of a $n$-tuple is synonymous to a [[Sequences|sequence]] of length $n$ which in itself is a function. Thus indeed every $n$ degree ordered pair can be represented as a function.
$$f:\{1\leq i \leq n\}\rightarrow\bigcup X_i:i\mapsto x_i\;\land\;x_i \in X_i \iff (f(i))_{i\in\mathbb{N}}^n=(f(1),...,f(i),...,f(n))\iff (x_1,...,x_i,...x_n)$$
This small demonstration is informal so we are going to formalize it a bit. We can define the $n$-tuple to be a surjective function whose range is an arbitrary set.
$$x:\{i\in\mathbb{N}:1\leq i \leq n\}\rightarrow A$$
$x$ has to be surjective because if not, one could enlarge the domain and have a function $\bar{x}$ that for every $i$ in the domain still has the same mapping as $x$. But this is a serious problem as we would lose the uniqueness of our representation. We would have 1 $n$-tuple that can be represented by an infinite amount of variations of $x$, we thus require the function $x$ to be surjective.

We then denote that $x_i=x(i)$ and that $x=(x_i)_{1\leq i\leq n}$. Once again we can verify that the property of equality at the start of the note still holds, thus giving us a valid definition.


