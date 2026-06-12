---
tags:
  - Area/Math/Geometry/Manifold/DifferentialManifold
  - Area/Math/Algebra
---
Let $M$ be a [[Differential Manifold|differential manifold]] and $\gamma,\gamma':\mathbb{R}\to M$ be [[Differential Manifold#Related concepts|curves]] on it. Let $x=\gamma(0)$, there is a [[Equivalence Relation|equivalence relation]] defined by
$$\frac{\mathrm{d}}{\mathrm{d}t}(\gamma \circ \phi ^{-1})\Bigg|_{t=0}=\frac{\mathrm{d}}{\mathrm{d}t}(\gamma' \circ \phi ^{-1})\Bigg|_{t=0}$$
for the chart $(U,\phi)$ where $x\in U$. A **tangent vector** at $x$ is an [[Equivalence Class|equivalence class]] of this relation. For curves that parameterized by $t$, we simply denote the tangent vector with $\mathrm{d} /\mathrm{d}t$. The set of all tangent vector at $x$ is denoted $T_{x}M$, called the **tangent space** at $x$. The tangent space is a [[Vector Space|vector space]] with the same dimension of the manifold.

In terms of local coordinate, the tangent vector can be expanded with differential w.r.t. $x^{\mu}$:
$$\frac{\mathrm{d}}{\mathrm{d}t}=\frac{\mathrm{d}x^{\mu}}{\mathrm{d}t} \frac{\partial }{\partial x^{\mu}}.$$
Thus one can regard $\partial_{\mu}=\partial /\partial x^{\mu}$ as a basis of tangent space, i.e. the **coordinate basis**.


## Related concepts
### Cotangent space & tensor space
Since $T_{x}M$ is a vector space, there exists a [[Dual Space|dual space]] to $T_{x}M$, such space is denoted $T_{x}^{*}M$, called **cotangent space**. The corresponding coordinate basis for cotangent space is $\mathrm{d}x^{\mu}$. Built from tangent space and cotangent space, then **$(r,s)$-tensor space** is the product 
$$T^{(r,s)}_{x}M=\otimes ^{r}T_{x}M\otimes ^{s}T_{x}^{*}M.$$
The coordinate basis is $\partial _{\mu_{1}}\cdots\partial _{\mu_{r}}\mathrm{d}x^{\nu_{1}}\cdots \mathrm{d}x^{\nu_{s}}$.

### Lie brackets of vectors
For $X,Y\in T_{x}M$, the **Lie brackets** for them is $[X,Y]\in T_{x}M$ such that
$$[X,Y](f)=X(Y(f))-Y(X(f)).$$