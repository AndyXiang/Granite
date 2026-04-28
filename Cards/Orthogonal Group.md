---
tags:
  - Area/Math/Algebra/Group/LieGroup
---
The **orthogonal group** of degree $n$ over field $\mathbb{K}$ is the [[Lie Subgroup|Lie subgroup]] of the [[General Linear Group|general linear group]] $\mathrm{GL}(n,\mathbb{K})$ as
$$\mathrm{O}(n,\mathbb{K})=\{ q:q^{\mathsf{T}}q=1_{n\times n} \}.$$
Usually one works in $\mathbb{R}$ and denote $\mathrm{O}(n,\mathbb{R})=\mathrm{O}(n)$. The **special orthogonal group** $\mathrm{SO}(n,\mathbb{K})$ is defined with extra condition
$$\mathrm{SO}(n,\mathbb{K})=\{ q:q\in\mathrm{O}(n,\mathbb{K}),\det(q)=1 \}.$$

## Properties
### Parameterization
There is a special element $p=\mathrm{diag}(-1,1,\cdots,1)\in \mathrm{O}(n)$, such that
$$\mathrm{O}(n)\cong \mathrm{\mathrm{SO}}(n)\cup p\mathrm{SO}(n).$$
So any parameterization of $\mathrm{SO}(n)$ directly leads to parameterization of $\mathrm{O}(n)$. To parameterize $\mathrm{SO}(n)$, one needs $n(n-1) /2$ parameters.

As [[Topological Manifold|manifolds]], no single global [[Z Coordinate System|coordinate chart]] can parameterize $\mathrm{\mathrm{SO}}(n)$ and $\mathrm{O}(n)$. As consequence, in practice one uses surjective parameterizations (often redundant) or charts valid on a [[Topological Space|open dense set]].

#### With exponential map
As a Lie group, one can construct the group $\mathrm{SO}(n)$ from its [[Lie Algebra|Lie algebra]] $\mathfrak{so}(n)$ with [[Lie Algebra|exponential map]]
$$q=\exp(x),x^{\mathsf{T}}=-x.$$
This is surjective, and far from [[Map#Properties|injection]].

#### Euler angles
Any $q\in \mathrm{SO}(n)$ ($n\geq2$) can be written as a product of some "elementary" plane rotations
$$q=\prod_{1\leq i<j\leq n}r_{ij}(\theta_{ij}),$$
where $r_{ij}(\theta_{ij})$ is identity except on the $(i,j)$-block where it equals to the 2D rotation matrix with angle $\theta_{ij}$. 

### Topology
 $\mathrm{O}(n)$ is [[Compact Space|compact]]. The [[Connected Space|connected component]] containing identity of $\mathrm{O}(n)$ is $\mathrm{SO}(n)$, thus $\mathrm{SO}(n)$ is connected.

For $n\geq2$, the [[Euler Characteristic|Euler characteristic]] $\chi(\mathrm{O}(n))=\chi(\mathrm{SO}(n))=0$. $\chi(\mathrm{O}(1))=\chi(\{ \pm1 \})=2,\chi(\mathrm{SO}(1))=\chi(\{ 1 \})=1$.

#### Lower dimensional topology
The low-dimensional (real) orthogonal groups are familiar [[Topological Space|spaces]]:
1. $\mathrm{O}(1)=\{ \pm1 \}$,
2. $\mathrm{SO}(1)=\{ 1 \}$,
3. $\mathrm{SO}(2)=\mathrm{S}^{1}$, the [[Sphere|1-sphere]].
4. $\mathrm{SO}(3)=\mathbb{RP}^{3}$, the 3-dimensional [[Projective Space|real projective space]], or say $\mathrm{S}^{3}$ identifying antipodal points.
5. $\mathrm{SO}(4)$ is [[Covering Space|doubly covered]] by $\mathrm{SU}(2)\times \mathrm{SU}(2)=\mathrm{S^{3}\times S^{3}}$.
#### Fundamental groups
The [[Homotopy Group|fundamental groups]] satisfy
$$\pi_{1}(\mathrm{O}(n))\cong \pi_{1}(\mathrm{SO}(n)).$$
We have
$$\pi_{1}(\mathrm{SO}(1))=0,\pi_{1}(\mathrm{SO}(2))\cong \mathbb{Z},\pi_{1}(\mathrm{SO}(n))\cong \mathbb{Z}_{2},n>2.$$

#### Universal covers
The [[Covering Space|double cover]] of $\mathrm{O}(n)$ is the [[Pin Group|Pin group]] $\mathrm{Pin}(n)$, and the double cover of $\mathrm{SO}(n)$ is $\mathrm{Sp in}(n)$ as the restriction along the inclusion $\mathrm{SO}(n)\hookrightarrow \mathrm{O}(n)$.

