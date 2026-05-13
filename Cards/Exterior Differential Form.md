---
tags:
  - Area/Math/Geometry/Manifold/DifferentialManifold
---
Let $M$ be a [[Differential Manifold|manifold]] and $x\in M$. A **exterior differential form** $\omega$ is a [[Fiber Bundle#Section|section]] of the [[Exterior Algebra|exterior algebra]] $\bigwedge T^{*}M$ of the [[Tangent Bundle|cotangent bundle]]. Conventionally, we denote the [[Vector Subspace|subspace]] $\bigwedge^{n}T^{*}M$  as $\Omega^{n}(M)$, whose elements are called **$n$-form**. 

In the [[Neighborhood|neighborhood]] $U \subset M$ with coordinates $\{ x_{i} \}$, a $n$-form can be expanded as
$$\omega=\frac{1}{n!}\sum_{i_{1},\cdots,i_{n}}\omega_{i_{1}\cdots i_{n}} \mathrm{d}x^{i_{1}}\wedge \cdots\wedge \mathrm{d}x^{i_{n}},$$
where $\omega_{i_{1}\cdots i_{n}}$ is a [[Smooth Mapping|smooth function]] over $M$. 

An unary operation $\mathrm{d}:\Omega^{r}(M)\to\Omega^{r+1}(M)$ is introduced as
$$\mathrm{d\omega}= \frac{1}{n!}\sum_{i_{1},\cdots,i_{n}}\mathrm{d}\omega_{i_{1}\cdots i_{n}}\wedge \mathrm{d}x^{i_{1}}\wedge \cdots\wedge \mathrm{d}x^{i_{n}}$$
for $\mathrm{d}\omega_{i_{1}\cdots i_{n}}\in T^{*}M$. This is called the **exterior derivative**.

