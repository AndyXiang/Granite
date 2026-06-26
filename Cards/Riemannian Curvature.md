---
tags:
  - Area/Math/Geometry/RiemannianGeometry
aliases:
  - Ricci Tensor
  - Torsion
  - Ricci Scalar
---
Let $M$ be a [[Riemannian Manifold|Riemannian manifold]] with metric $g$ and [[Affine Connection|metric connection]] $\nabla$. The **Riemannian curvature** $R:\mathfrak{X}(M)\times\mathfrak{X}(M)\times\mathfrak{X}(M)\to\mathfrak{X}(M)$ is defined by
$$R(X,Y,Z)=\nabla(X,\nabla(Y,Z))-\nabla(Y,\nabla(X,Z))-\nabla([X,Y],Z).$$
The **torsion** $T:\mathfrak{X}(M)\times \mathfrak{X}(M)\to \mathfrak{X}(M)$ is defined by
$$T(X,Y)=\nabla(X,Y)-\nabla(Y,X)-[X,Y].$$


In coordinates, one has
$$R^{\kappa}_{~~\lambda \mu \nu}=\partial _{\mu}\Gamma^{\kappa}_{~~\nu\lambda}-\partial _{\nu}\Gamma^{\kappa}_{~~\mu\lambda}+\Gamma^{\eta}_{~~\nu\lambda}\Gamma^{\kappa}_{~~ \mu \eta}-\Gamma^{\eta}_{~~\mu\lambda}\Gamma^{\kappa}_{~~ \nu \eta}$$
where $\Gamma^{\kappa}_{~~\mu \nu}$ is connection coefficients. **Ricci tensor** is defined by $R_{\mu \nu}=R^{\kappa}_{~~\mu\kappa \nu}$ and **Ricci scalar** is defined by $R=g^{\mu \nu}R_{\mu \nu}$.

1. $R^{\kappa}_{~~\lambda \mu \nu}=-R^{\kappa}_{~~\lambda \nu \mu}$.