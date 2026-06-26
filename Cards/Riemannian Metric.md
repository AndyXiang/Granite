---
tags:
  - Area/Math/Geometry/Manifold/DifferentialManifold
  - Area/Math/Geometry/RiemannianGeometry
---
Let $M$ be a [[Differential Manifold|differential manifold]]. A **Riemannian metric** $g$ is a rank $(0,2)$ [[Tangent Bundle|tensor field]] over $M$ that satisfies
1. *symmetric*: $g(x,y)=g(y,x)$, for all [[Tangent Bundle|vector fields]] $x,y\in \mathfrak{X}(M)$.
2. *non-negative*: $g(x,x)\geq 0$, for all [[Tangent Bundle|vector fields]] $x\in \mathfrak{X}(M)$, where equality holds only for $x=0$.

A **pseudo-Riemannian metric** $g$ is a rank $(0,2)$ tensor field that is symmetric and satisfies $\forall x\in TM,g(x,y)=0\implies y=0$.

Since (pseudo-)Riemannian metric is symmetric, one can always diagonalize it on a chart $U$ with some coordinates $\{ x^{\mu} \}$:
$$g=g_{\mu \nu}\mathrm{d}x^{\mu}\otimes \mathrm{d}x^{\nu}$$
where $g_{\mu \nu}$ is a diagonalized matrix with eigenvalues being $\pm 1$. The numbers of positive and negative eigenvalues $(i, j)$ are called the **index** of the metric. There are some special cases:
1. **Euclidean metric**: $j=0$, such that $g_{\mu \nu}=\delta_{\mu \nu}=\mathrm{diag}(1,1,\cdots, 1)$.
2. **Minkowski metric**: $j=1$, such that $g_{\mu \nu}=\eta_{\mu \nu}=\mathrm{diag}(-1,1,1,\cdots,1)$.


## Induced metric
Let $M$ be a differential manifold with metric $g$. Let $N$ be its [[Submanifold|submanifold]] with embedding $f:N\to M$. The pull-back $f^{*}$ induces a metric on $N$ as
$$\tilde{g}_{\mu \nu}\big|_{p}=g_{\alpha\beta}\big|_{f(p)} \frac{\partial f^{\alpha}}{\partial x^{\mu}} \frac{\partial f^{\beta}}{\partial x^{\nu}}.$$
Then $\tilde{g}=\tilde{g}_{\mu \nu}\mathrm{d}x^{\mu} \otimes \mathrm{d}x^{\nu}$ is called the **induced metric** on $N$.