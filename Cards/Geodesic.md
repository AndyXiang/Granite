---
tags:
  - Area/Math/Geometry/RiemannianGeometry
---
Let $M$ be a [[Riemannian Manifold|Riemannian manifold]] and $\nabla$ be an [[Affine Connection|affine connection]] over $M$. Let $c:\mathbb{R}\to M$ be a [[Differential Manifold|curve]] (assume it's covered in one chart $(U,\varphi)$ for simplicity). A vector field $x\in \mathfrak{X}(M)$ is said to be **parallel transported** along $c$ iff
$$\nabla(v,x)=0$$
where $v=\mathrm{d} /\mathrm{d}t$ is the [[Tangent Space|tangent vector]] of $c$. If the tangent vector itself is parallel transported along the curve, the curve is called a **geodesic**, that is
$$\nabla(v,v)=0.$$

In coordinates, the equation for geodesic is
$$\frac{\mathrm{d}^{2}x^{\lambda}}{\mathrm{d}t^{2}}+\Gamma^{\lambda}_{~~\mu \nu} \frac{\mathrm{d} x^{\mu}}{\mathrm{d} t} \frac{\mathrm{d} x^{\nu}}{\mathrm{d} t}=0. $$