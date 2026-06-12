---
tags:
  - Area/Math/Geometry/RiemannianGeometry
---
Let $M$ be a [[Riemannian Manifold|Riemannian manifold]] with metric $g$ and [[Affine Connection|metric connection]] $\nabla$. The **Riemannian curvature** $R:\mathfrak{X}(M)\times\mathfrak{X}(M)\times\mathfrak{X}(M)\to\mathfrak{X}(M)$ is defined by
$$R(x,y,z)=\nabla(x,\nabla(y,z))-\nabla(y,\nabla(x,z))-\nabla([x,y],z).$$

In coordinates, one has
$$R^{\kappa}_{~~\lambda \mu \nu}=\partial _{\mu}\Gamma^{\kappa}_{~~\nu\lambda}-\partial _{\nu}\Gamma^{\kappa}_{~~\mu\lambda}+\Gamma^{\eta}_{~~\nu\lambda}\Gamma^{\kappa}_{~~ \mu \eta}-\Gamma^{\eta}_{~~\mu\lambda}\Gamma^{\kappa}_{~~ \nu \eta}$$
and $R^{\kappa}_{~~\lambda \mu \nu}=-R^{\kappa}_{~~\lambda \nu \mu}$.