---
tags:
  - Area/Math/Geometry/Manifold/DifferentialManifold
  - Area/Math/Analysis/MeasureTheory
  - Area/Math/Topology
  - Area/Math/Algebra/Group
---
Let $G$ be a [[Z σ-Compact Space|σ-compact]] [[Z Locally Compact Space|locally compact]] [[Hausdorff Topological Space|Hausdorff]] [[Topological Group|group]]. The **left Haar measure** is a non-zero [[Radon Measure|Radon measure]] that is left-invariant:
$$\mu(gE)=\mu(E)$$
for all $g\in G$ and [[Borel Measure|Borel measurable]] sets $E$. The right Haar measure is defined similarly.

>[!tip] Existence and Uniqueness
>Let $G$ be a $\sigma$-compact locally compact Hausdorff group. Then there exists a left Haar measure $\mu$ on $G$. Further more, this measure is unique up to scalars; that is, for two left Haar measure $\mu,\nu$, then $\mu=\lambda \nu$ for some $\lambda>0$.

## Examples
1. [[Z Lebesgue Measure|Lebesgue measure]] is a left Haar measure on Euclidean spaces $\mathbb{R}^{d}$ as the group of addition.
2. If $G$ is a countable discrete group, then the measure by counting is a left and right Haar measure.

## Computations
For simplicity, here we discuss the case that $G$ is a [[Lie Group|Lie group]]. The main idea to compute the Haar measure is to take a [[Exterior Differential Form|volume form]] and solve a coefficient that makes the corresponding measure left (or right) invariant. In formula, this is
$$\mu(g)=\mu(gh)=\lambda(h)^{*}\mu(g)$$
where $\lambda(h)^{*}$ is the pullback for functions $\mathfrak{C}^{\infty}(G)\to \mathfrak{C}^{\infty}(G)$.

To be explicit, let $x^{\mu}$ be the local coordinates of the neighborhood of identity, and $y^{\mu}$ the coordinates around some group element $h$. So the Haar measure near $e$ is $\mu(g)=E(x)\mathrm{d}x$, and $\mu(g)=H(y)\mathrm{d}y$ near $h$, where $\mathrm{d}x=\mathrm{d}x^{1}\wedge \cdots \wedge \mathrm{d}x^{n}$ and $\mathrm{d}y=\mathrm{d}y^{1}\wedge \cdots \wedge \mathrm{d}y^{n}$ are the volume forms. We choose a normalization that $E(e)=1$. In these coordinates, the pull-back is the [[Z Jacobian|Jacobian]]
$$\lambda(h)^{*}=\det\left(  \frac{\partial y}{\partial x} \right)_{h}.$$
Thus the coefficient $H(y)$ satisfies
$$\left|H(y)\det\left(  \frac{\partial y}{\partial x} \right)_{h}\right|=1.$$
Finally, the left Haar measure around $h$ is
$$\mu(g)=\left|\det\left(  \frac{\partial y}{\partial x} \right)_{h}\right|^{-1} \mathrm{d}y$$

Another way to compute it is by computing the [[Maurer-Cartan Form|Maurer-Cartan form]], which also encodes the left-invariance. Use the definition
$$\omega=g^{-1}\mathrm{d}g=\omega_{a}t^{a},$$
where $t^{a}$ is basis of the [[Lie Algebra|Lie algebra]] $\mathfrak{g}=T_{e}G$. Every $\omega_{a}$ is a left-invariant [[Exterior Differential Form|1-form]], so
$$\mu=\omega^{1}\wedge \cdots\wedge\omega^{n}$$
is a left Haar measure.