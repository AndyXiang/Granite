---
tags:
  - Area/Math/Geometry/RiemannianGeometry
---
Let $M$ be a [[Differential Manifold|differential manifold]]. An **affine connection** on $M$ is a map $\nabla:\mathfrak{X}(M)\times \mathfrak{X}(M)\to \mathfrak{X}(M)$ satisfies
1. *bilinearity*: $\nabla(ax+by,cz+dw)=ac\nabla(x,z)+ad\nabla(x,w)+bc\nabla(y,z)+bd\nabla(y,w)$, for all $x,y,z,w\in \mathfrak{X}(M)$ and $a,b,c,d\in \mathbb{R}$.
2. $\nabla(fx,y)=f\nabla(x,y)$, for every $x,y\in \mathfrak{X}(M),f\in \mathfrak{C}^{\infty}(M)$.
3. $\nabla(x,fy)=x(f)y+f\nabla(x,y)$, for every $x,y\in \mathfrak{X}(M),f\in \mathfrak{C}^{\infty}(M)$.

Take a chart $(U,\varphi)$ with coordinates $\{ x^{\mu} \}$, the **connection coefficients** are
$$\nabla(e _{\mu},e _{\nu})=e _{\lambda}\Gamma^{\lambda}_{~~\mu \nu},$$
where $\{ e_{\mu}=\partial /\partial x^{\mu} \}$ is the basis of $T_{U}M$. With these, one can expand as
$$\nabla(x,y)=x^{\mu}y^{\nu}\Gamma^{\lambda}_{~~\mu \nu}e_{\lambda}.$$