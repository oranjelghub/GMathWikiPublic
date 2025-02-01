
In addition to the basic operations of [[Union, intersection and difference of sets|union]], [[Union, intersection and difference of sets|intersection]], and [[Union, intersection and difference of sets|differencing]], another fundamental operation on [[Sets|sets]] is that of the Cartesian product.

If $X$ and $Y$ are sets, then we define the Cartesian product $X \times Y$ to be the collection of ordered pairs, whose first component lies in $X$ and second component lies in $Y$ , thus:
$$X \times Y:=\{(x,y):x\in X, y \in Y\}$$
or equivalently
$$a\in (X \times Y)\iff (a = (x, y) \;\text{for some}\; x ∈ X \;\text{and}\; y ∈ Y )$$

We somewhat axiomatically defined the existence of the cartesian product of two sets. In order to avoid adding more axioms to the list we can actually proof the existence of the cartesian product by first redefining the notion of a two fold ordered pair.
$$(x,y):=\{\{x\},\{x,y\}\}$$
From this follows the proof


#### *Proof*

Suppose we have two sets $X$ and $Y$, according to the power set axiom and the axiom of pairing we know that the following set exists:
$$\mathcal{P}(\mathcal{P}(X\cup Y))$$
We can now apply the axiom of specification on this set, we will namely construct $\{\alpha\in \mathcal{P}(\mathcal{P}(X\cup Y)):\alpha=\{\{x\},\{x,y\}\}\land x\in X,y\in Y\}$. One can then easily show that $X\times Y$ is equal to that set, proving it's existence.

**Q.E.D.**

Alternatively I came up with this definition before finding this easier one.
$$\bigcup_{y\in Y}X\times\{y\}\;\text{with}\;X\times\{y\}=\{(x,y):P(x,y)\;\text{and}\;x\in X\}\;\text{with}\;P:(x,y)=\{x,\{x,y\}\}$$
One can easily check those sets are synonymous.

## *$n$ fold cartesian product*

We can extend this notion of cartesian product between 2 sets to the cartesian product of $n$ sets: If $(X_i)_{1≤i≤n}$ is an [[Ordered pairs and n-tuples|ordered n-tuple]] of sets, we define their Cartesian product $\Pi_{1≤i≤n} X_i$ (also denoted $\prod^n_{i=1} X_i$ or $X_1 \times ... \times X_n$) by: 
$$\prod_{1\leq i \leq n}X_i := \{(x_i)_{1 \leq i \leq n}:x_i \in X_i \,, 1\leq i \leq n\}$$
We can also prove that $\prod_{1\leq i \leq n}X_i$ is indeed a set, which we do down in the note.

An ordered $n$-tuple $x_1,...,x_n$ of objects is also called an ordered sequence of $n$ elements, or a finite sequence for short. Also, the empty Cartesian product $\prod_{1≤i≤0} X_i$ gives, not the empty set $\{\}$, but rather the singleton set $\{()\}$ whose only element is the 0-tuple $()$, also known as the empty tuple.


#### *Proof*

From the power set axiom we can construct the set of functions with domain $\{1\leq i \leq n\}$ and range $\bigcup_{1\leq i \leq n}X_i$. Now by axiom of specification we construct a set such that we have all these functions but only the ones that map $i\mapsto x_i$ and $x_i\in X_i$ for all $1\leq i\leq n$: 
$$\left\{f:f(i)=x_i \land x_i\in X_i \land f \in \{1\leq i\leq n\}^{\bigcup_{1\leq i\leq n}X_i}\right\}$$
By axiom of replacement we build a set that replaces every $f$ by it's partial function set $F$
$$\left\{F:F\; \text{is the set of all partial functions of}\;f\land f\in\left\{f:f(i)=x_i \land x_i\in X_i \land f \in \{1\leq i\leq n\}^{\bigcup_{1\leq i\leq n}X_i}\right\}\right\}$$
Since this is a set of sets we just take the arbitrary union, so we obtain an set of all different functions with a different mapping, from which some of them have the same mapping but a different domain and/or range (There is no overlap between the set of partial functions $F_k\cap F_l=\emptyset$). We now apply the axiom of specification in order to filter out all the non-surjective functions.
$$\left\{\tilde{f}\;\text{is surjective}\land \tilde{f}\in\bigcup\left\{F:F\; \text{is the set of all partial functions of}\;f\land f\in\left\{f:f(i)=x_i \land x_i\in X_i \land f \in \{1\leq i\leq n\}^{\bigcup_{1\leq i\leq n}X_i}\right\}\right\}\right\}$$
Thus giving us a set of functions which are all surjective (Little sidenote: every $f$ has only one surjective variant, because if there were more then the functions would be equal) and all map $i$ to $x_i$ with $x_i\in X_i$. But according to an alternative definition of [[Ordered pairs and n-tuples|n-tuples]] these functions are all unique representations of a specific $n$-tuple and thus we just built a set of all $n$-tuples where every $x_i$ is a member of the set $X_i$. Which proves that we can indeed construct the set $\prod_{1\leq i\leq n}X_i$ and that it is indeed a perfectly valid set.

**Q.E.D.**
## *Finite choice* 

Let $n ≥ 1$ be a natural number, and for each natural number $1 ≤ i ≤ n$, let $X_i$ be a non-empty set. Then there exists an $n$-tuple $(x_i)_{1≤i≤n}$ such that $x_i \in X_i$ for all $1 ≤ i ≤ n$. In other words, if each $X_i$ is non-empty, then the set $\prod_{1≤i≤n} X_i$ is also non-empty.

This notion was already discussed and proven in the note over [[Sets|sets]] but we will want to now extend this notion to $n$ elements and sets.

#### *Proof*

We induct on $n$ (starting with the base case $n = 1$; the claim is also vacuously true with $n = 0$ but is not particularly interesting in that case). When $n = 1$ the claim follows from a lemma proven in the note about [[Sets|sets]]. Now suppose inductively that the claim has already been proven for some $n$; we will now prove it for $S(n)$. Let $X_1,...,X_{S(n)}$ be a collection of nonempty sets. By induction hypothesis, we can find an $n$-tuple $(x_i)_{1≤i≤n}$ such that $x_i ∈ X_i$ for all $1 ≤ i ≤ n$. Also, since $X_{S(n)}$ is non-empty, by lemma we may find an object $a$ such that $a ∈ X_{S(n)}$. If we thus define the $S(n)$-tuple $(y_i)_{1≤i≤S(n)}$ by setting $y_i := x_i$ when $1 ≤ i ≤ n$ and $y_i := a$ when $i = S(n)$ it is clear that $y_i ∈ X_i$ for all $1 ≤ i ≤ S(n)$, thus closing the induction.

**Q.E.D.**


#completed 


