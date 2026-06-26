---
tags:
  - Area/Math/Geometry/RiemannianGeometry
aliases:
  - Covariant Derivative
---
Let $M$ be a [[Differential Manifold|differential manifold]]. An **affine connection** on $M$ is a map $\nabla:\mathfrak{X}(M)\times \mathfrak{X}(M)\to \mathfrak{X}(M)$ satisfies
1. *bilinearity*: $\nabla(aX+bY,cZ+dW)=ac\nabla(X,Z)+ad\nabla(X,W)+bc\nabla(Y,Z)+bd\nabla(Y,W)$, for all $X,Y,Z,W\in \mathfrak{X}(M)$ and $a,b,c,d\in \mathbb{R}$.
2. $\nabla(fX,Y)=f\nabla(X,Y)$, for every $X,Y\in \mathfrak{X}(M),f\in \mathfrak{C}^{\infty}(M)$.
3. $\nabla(X,fY)=X(f)Y+f\nabla(X,Y)$, for every $X,Y\in \mathfrak{X}(M),f\in \mathfrak{C}^{\infty}(M)$.

Take a chart $(U,\varphi)$ with coordinates $\{ x^{\mu} \}$, the **connection coefficients** are
$$\nabla(e _{\mu},e _{\nu})=e _{\lambda}\Gamma^{\lambda}_{~~\mu \nu},$$
where $\{ e_{\mu}=\partial /\partial x^{\mu} \}$ is the basis of $T_{U}M$. With these, one can expand as
$$\nabla(X,Y)=X^{\mu}\left( \frac{\partial Y^{\lambda}}{\partial x^{\mu}}+\Gamma^{\lambda}_{~~\mu \nu}Y^{\nu} \right)e_{\lambda}.$$

By requiring that $\nabla(X,f)=X(f)$ for $X\in \mathfrak{X}(M),f\in \mathfrak{C}^{\infty}(M)$, one can extend the definition of affine connection to $\nabla:\mathfrak{X}(M)\times T^{(r,s)}M\to T^{(r,s)}M$ for any $r,s\in \mathbb{N}$ that satisfies bilinearity and Leibnitz law:
$$\nabla(X,T_{1}\otimes T_{2})=\nabla(X,T_{1})\otimes T_{2}+T_{1}\otimes \nabla (X,T_{2}).$$

## Christoffel symbol
$${ \kappa \brace \mu~\nu }=\frac{1}{2}g^{\kappa\lambda}(\partial _{\mu}g_{\lambda \nu}+\partial _{\nu}g_{\lambda \mu}-\partial _{\lambda}g_{\mu \nu}) $$
where $g$ is the [[Riemannian Metric|metric]]. Define **torsion** $T^{\rho}_{~~\mu \nu}=2\Gamma^{\rho}_{~~[\mu \nu]}$. The connection satisfies
$$\Gamma^{\lambda}_{~~\mu \nu}= {\lambda \brace \mu~ \nu }+T^{\lambda}_{~~\mu \nu}$$
