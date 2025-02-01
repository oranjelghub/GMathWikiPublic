---
Date created: 2024-09-28 13:46
tags:
  - Type/Refined_Note
  - Topic/Physics
---

---

Types: _Not applicable_
Examples: [[Center of mass in a semi circle with uniform density]]
Properties: [[Partitioning of continuous systems with uniform density for easier computing of the center of mass]]

Justifications: [[Center of mass in a discrete system]]
Specializations: [[Center of mass in a discrete system]]
Generalization: [[Center of mass in a continuous 3 dimensional system with variable density]]

---

Let $Q\subset \mathbb{R}^{3}$ be a a continuous system of particles$^{[1]}$ with total mass $M$ and volume $V_{A}$ and uniform density $\rho$, noting that per definition of density $dm=\rho  dV$. We now generalize the center of mass from a discrete system to a continuous system by $$ \sum^{k}_{i=1}m_{i}(p_{i}-R)\longrightarrow \int_{} \int_{} \int_{Q} (r-R)\rho \;dV=0$$Where the particles $p_{i}$ with their respective weight $m_{i}$ become$^{[2]}$ arbitrary particles $r$ with their respective infinitesimal weight $dm$. 

>[!quote]- Working out $R$ from $\int_{} \int_{} \int_{Q} (r-R)\rho \;dV=0$
>We now want to compute $R$, so we first split up the integral like this $$ \int_{} \int_{} \int_{Q} r\rho \;dV=\int_{} \int_{} \int_{Q} R\rho \;dV$$We can then pull out the constant $R$ and $\rho$ $$ \int_{} \int_{} \int_{Q} r\rho \;dV=R\rho\int_{} \int_{} \int_{Q}  \;dV $$ But you will notice that $\int_{}\int_{}\int_{Q}\;dV$ is just the total volume of $Q$, which once multiplied by $\rho$ gives us the total mass of $Q$, namely $M$. It follows that $$ R=\frac{1}{M} \int_{} \int_{} \int_{Q} r\rho\; dV$$

Do note that $r$ is considered a variable in this context, whilst $R$ is some fixed point or in other words a constant. Notice that if we are also not in three dimensions, but two for example, that our triple integral becomes a double integral. For example in 2d we search a point $R$ that satisfies $$ \int_{} \int_{Q} (r-R)\rho \;dA $$

---

**_Remark_**$^{[1]}$: For the sake of ease we will not define what a continuous system of particles is, and just let our intuition speak regarding the type of systems we are studying. If you want examples, think any standard solid for example, like a sphere or cube or triangle etc...

**_Remark_**$^{[2]}$: Since this is physics and not mathematics we can do the transition from a sum to an integral in this hand-wavery manner without bothering with the associated formalities. As rule of thumb, in physics we may often make the following transform $$ \sum^{}_{}\Delta x \longrightarrow \int_{} \;dx$$