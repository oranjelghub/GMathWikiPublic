---
Date created: 2024-09-26 21:38
tags:
  - Type/Lecture_Note
  - Topic/Physics
---
---

There are two types of quantities we distinguish in physics, namely scalar and vectorial.
- Scalars are simple $\lambda\in \mathbb{R}$
- Vectors are objects $v\in \mathbb{R}^{n}$

---

We denote the magnitude of a real vector by $$ v=\left|\vec{v}  \right|=\left| \left| \vec{v} \right|  \right|   $$If $v\in \mathbb{R}^{2}$, we may represent $\vec{v}$ by the pair defined by its magnitude and the angle it makes with the $x$-axis $$ (v_{x},v_{y})=(v\cos(\theta),v\sin(\theta)) $$If instead we are talking about a vector between two points $P_{1}=(x_{1},y_{1})$ and $P_{2}=(x_{2},y_{2})$, we define $$ \vec{P_{1}P_{2}}:=(x_{2}-x_{1},y_{2}-y_{1}) $$With all these vectors, we use the stander vector space algebra of $\mathbb{R}^{n}$.

---

We can use the right hand rule to determine the exact position and direction of a $z$-axis, given a $x$-axis and $y$-axis.

---

We define the magnitude or norm of some $\vec{v}\in \mathbb{R}^{n}$ with coordinates $(x_i)^n_{i=1}$ by $$ v=\left| \vec{v} \right| :=\sqrt{ \sum^{n}_{i=1}x^{2}_{i} } $$We say that a vector $\vec{e}$ is a unit vector iff $e=1$. If we take the standard orthogonal and orthonormal basis for $\mathbb{R}^{n}$, we may write every vector $\vec{v}\in \mathbb{R}^{n}$ with coordinates $(x_i)^n_{i=1}$ as $$ \vec{v}=\sum^{n}_{i=1}x_{i}\vec{e_{i}}$$

---

We define a product on the vectors of $\mathbb{R}^{n}$, namely the scalar product, define by $$ \vec{u}*\vec{v}:=\left| u \right| \left| v \right| \cos(\theta) $$Where $\theta$ is the angle they make. Notice that this product is exactly equal to zero when the vectors are orthogonal. The following properties also follow from this definition: 
- Commutativity
- Distributivity over addition
- Associativity and compatibility with standard scalar multiplication
- If $\theta=0$, then $\vec{a}*\vec{b}=ab$
- If $\theta=\pi$, then $\vec{a}*\vec{b}=-ab$
Now remember since we can write $\vec{v}=\sum^{n}_{i=1}x_{i}\vec{e_{i}}$, it follows by the previous properties that $$ \vec{v}*\vec{u}=\sum^{n}_{i=1}x_{i}y_{i} $$
---

We can also determine the norm of a sum of vectors by defining $\vec{c}:=\vec{a}+\vec{b}$, then $$ \begin{align} \vec{c}*\vec{c}=c^{2}&=(\vec{a}+\vec{b})(\vec{a}+\vec{b})\\&=\vec{a}*\vec{a}+\vec{b}*\vec{b}+2\vec{a}*\vec{b}\\&=a^{2}+b^{2}+2ab\cos(\theta)\\c&=\sqrt{ a^{2}+b^{2}+2ab\cos(\theta) }\end{align}$$

---

We also define the vector product for two vectors $\vec{v},\vec{u}\in \mathbb{R}^{n}$ by $$ \vec{v}\times \vec{u}:=\left| \vec{v} \right| \left| \vec{u} \right| \sin(\theta)\vec{p} $$Where $\vec{p}$ is some vector perpendicular to the plane spanned by $\vec{v}$ and $\vec{u}$. Note that vector multiplication is **NOT COMMUTATIVE**. Some important properties that follow:
- Given any basis vector of $\mathbb{R}^{3}$$$ \vec{e}\times \vec{e}=0 $$
- Given any two basis vectors of $\mathbb{R}^{3}$ (toemaatje: $x\to y\to z$) $$ \begin{align} \vec{e}_{x}\times \vec{e}_{y}&=\vec{e}_{z}\\ \end{align} $$
Now remember since we can write $\vec{v}=\sum^{3}_{i=1}v_{i}\vec{e_{i}}$ for $\vec{v}\in \mathbb{R}^{3}$, it follows by the previous properties that 
$$ \vec{v}\times \vec{u}=\det \left( \begin{bmatrix} v_{y}&v_{z}\\u_{x}&u_{z}
\end{bmatrix} \right)\vec{e}_{x}+\det \left( \begin{bmatrix}
v_{x}&v_{y}\\u_{x}&u_{y}\end{bmatrix} \right) \vec{e}_{y}+\det \left( \begin{bmatrix}
v_{x}&v_{z}\\u_{x}&u_{z}\end{bmatrix} \right)\vec{e}_{z}   $$

---

A line between two points $A$ and $B$ both in $\mathbb{R}^{n}$ can be constructed by considering $$ L:=\left\{ A+\lambda(B-A) \}:\lambda\in[0,1] \right\}  $$
