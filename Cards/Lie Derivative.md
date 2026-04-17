---
tags:
  - Area/Math/Geometry/Manifold/DifferentialManifold
---
Given a [[Differential Manifold|smooth manifold]] $M$ and a [[Tangent Bundle|smooth vector field]] $X\in \mathfrak{X}(M)$, the **Lie derivative** $\mathcal{L}_{X}$ is a series of operators on the spaces of [[Differential Form|differential forms]], of [[Function|functions]], and other [[Tensor Field (Manifold)|tensor fields]]. 
1. Functions: $\mathcal{L}_{X}:\mathfrak{C}^{\infty}(M)\to \mathfrak{C}^{\infty}(M)$, for $f\in \mathfrak{C}^{\infty}(M)$, $\mathcal{L}_{X}f$ is the function satisfying $$(\mathcal{L}_{X}f)(p)=\frac{\mathrm{d}}{\mathrm{d}t}\bigg|_{t=0}(f\circ\gamma_{X}^{t})(p),$$ where $\gamma_{X}^{t}:\mathbb{R}\times M\to M$ is the [[Flow (Manifold)|flow]] of vector field $X$.
2. Vector fields: $\mathcal{L}_{X}:\mathfrak{X}(M)\to \mathfrak{X}(M)$ as $\mathcal{L}_{X}Y=[X,Y],Y\in \mathfrak{X}(M)$, where $[X,Y]\in \mathfrak{X}(M)$ is the [[Tangent Space|Lie bracket of vectors]]. 
3. Differential forms: $\mathcal{L}_{X}:\Omega^{*}(M)\to \Omega^{*}(M)$, for $\omega\in\Omega^{*}(M)$, $\mathcal{L}_{X}\omega$ is the pullback of $\omega$ along the flow of $X$: $$\mathcal{L}_{X}\omega=\frac{\mathrm{d}}{\mathrm{d}t}\bigg|_{t=0}(\gamma_{X}^{t})^{*}(\omega).$$
