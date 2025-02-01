## *Definition*

The polar coordinate system is a two-dimensional coordinate system in which each point on a plane is determined by a distance from a reference point and an angle from a reference direction. The reference point (analogous to the origin of a [[Cartesian coordinate system]] is called the pole, and the ray from the pole in the reference direction is the polar axis. The distance from the pole is called the radial coordinate, radial distance or simply radius, and the angle is called the angular coordinate or polar angle.

$$(x,y) \longrightarrow (r, \theta) $$
Since the radius $r$ is defined as the distance from the pole we also note that $r \geq 0$ .
We must also note that in polar coordinates the following holds: $$\forall P\in \mathbb{R}^2: (r,\theta)=(r, \theta +k2\pi): k \in\mathbb{Z}$$Thus we can restrict the polar angle such that $$\theta \in \left[ 0,2\pi  \right[$$
We also note that the origin or pole has even more equivalent points.

![[Polar grid 1.png|300]]


We will also denote the set $P$, which is the set of all polar coordinates and is defined by a [[Cartesian product]] as: $$P:= \mathbb{R}^+ \times \mathbb{R}^+ $$
We choose this definition because we consider distance and angles to be only positively valued concepts here. This also means that $$P\subset\mathbb{R}^2$$






#### Short trivial proof 

$$\forall(r,\theta) \in P:r,\theta\in\mathbb{R}^+ \implies r,\theta\in\mathbb{R}\implies(r,\theta)\in \mathbb{R}^2 \implies P \subset \mathbb  {R}^2$$

**Q.E.D.**
## *Maps between coordinate systems*


#### *Mapping between cartesian plane and polar plane*


##### $\mathbb{R}^2$ to polar

In order to construct a map we will need to be careful with certain subtleties. First of all the angles are equivalent op to multiples of $2\pi$ and thus we will need to define a parametric map. Giving a one closed formula for the angle will also not be possible, as the method of calculation depends on the signs of $(x,y)$. So we will first pose a angle or theta [[Functions|function]]: $$\Theta:\mathbb{R}^2\longrightarrow\mathbb{R}:(x,y)\longmapsto
\left\{ \begin{align}
\arctan(\frac{y}{x}) \hspace{1cm} &:x>0 \\
\pi+\arctan(\frac{y}{x}) \hspace{1cm}&:x<0 \\
\frac{\pi}{2} \hspace{1cm}&: x=0 \land y>0 \\
\frac{-\pi}{2} \hspace{1cm}&: x=0 \land y<0 \\
\text{undefined} \hspace{1cm}&:x=0\land y=0 \\
\end{align}\right.$$
We can now define the parametric map: 
$$ T_{\mathbb{R}^2\rightarrow P}^k:\mathbb{R}^2\longrightarrow \mathbb{R}^2:(x,y) \longrightarrow(\sqrt{x^2+y^2},\Theta(x,y)) $$
#comeback  and study properties of the [[Functions|function]]


##### Polar to $\mathbb{R}^2$

We define the following [[Functions|function]]: $$T_{P\rightarrow \mathbb{R}^2}:\mathbb{R}^2 \longrightarrow\mathbb{R}^2:(r,\theta)\longrightarrow(r\cos{\theta},r\sin{\theta})$$
We must also note that: $$\forall k \in \mathbb{Z}:T_{P\rightarrow \mathbb{R}^2}(r,\theta +k2\pi)=T_{P\rightarrow \mathbb{R}^2}(r, \theta)$$
This means this [[Functions|map]] is surjective. #comeback  study properties of the [[Functions|function]]



## *Polar equations*

A polar equation is an equation pertaining to polar coordinates under the form: $$f(r,\theta)=0$$
With this definition we can also define curves on the polar plane as [[Sets|sets]] or [[Functions|functions]].
$$r:\mathbb{R}^+ \longrightarrow\mathbb{R}^+:\theta\longrightarrow r(\theta) $$
$$\mathcal{C}=\left\{  (r,\theta)|(r,\theta) \in P \land f(r,\theta)=0  \right\}$$

#### *Cartesian to polar equations*

In order to transform a basic cartesian equation into a polar one we utilize the following fact:
$$
\left\{\begin{align}
x=r\cos(\theta) \\
y=r\sin(\theta) \\
\end{align}\right.
$$
And thus we can transform a cartesian [[Functions|function]] by simply replacing every $x$ and $y$
$$\left\{\begin{align}
f(x)&\rightarrow f(r\cos(\theta)) \\
f(x,y)&\rightarrow f(r\cos(\theta),r\sin(\theta))\\
\end{align}\right.
$$

#### *Symmetries of polar curves*

- If $r(-\theta)=r(\theta)$ then we have symmetry around the horizontal ray.
- If $r(\pi-\theta)=r(\theta)$ then we have a symmetry around the vertical ray.
- If $r(\alpha-\theta)=r(\theta)$ then we have a symmetry around the ray oriented $\alpha$ degrees from the pole.


#### *Intersection of polar curves*

#### *Examples of curves*

We will take a look at some explicit curves in polar form.


##### Circle
Main note: [[Circles]]

The equation of a circle with points $(r,\theta)$ in the polar plane with center $(r_0, \phi)$ and radius $a$ is: $$r^2-2rr_0\cos(\theta-\phi)+r_0^2=a^2$$For a generic circle centered around the pole with radius $a$ we get: $$r(\theta)=a$$

##### Line

Radial lines that pass through the pole with angle $\gamma$ are represented by the equation: $$\theta=\gamma$$
#comeback  For non radial lines


##### Polar rose
Main note [[Polar roses]]

A polar rose is a curve that looks like petalled flower and can be expressed with the following equation: $$r(\theta)=a\cos(k\theta+\gamma_0)$$
Here $a$ scales the size of the petals, $y_0$ provides a rotation around the pole and $k$ generates more petals. If $k$ is an integer then we will have $k$ petals if $k$ is odd or $2k$ petals if $k$ is even.

##### Archimedean spiral
Main note: [[Archimedean spiral]]

A spiral on the polar plane is described with the following equation: $$r(\theta)=a\theta+b$$$a$ scales the distance between loops, whilst $b$ moves the spiral along the imaginary horizontal axis.

## *Calculus on the polar plane*

