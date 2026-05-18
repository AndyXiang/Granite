---
tags:
  - Area/Math/Algebra/AssociativeAlgebra/ExteriorAlgebra
  - Area/Math/Algebra/VectorSpace
aliases:
  - Grassmann Algebra
---
Let $V$ be a [[Vector Space|vector space]] over [[Field (Math)|field]] $\mathbb{K}$. For vector space $V^{\otimes n}=\bigotimes_{i=1}^{n}V$, introduce the *anti-symmetrizer* $a:V^{\otimes n}\to V^{\otimes n}$ as
$$a=\frac{1}{n!}\sum_{\sigma\in S_{n}}\mathrm{sgn}(\sigma)\sigma$$
by the canonical action of [[Permutation Group|permutation group]] $S_{n}$ on $V^{\otimes n}$. Explicitly, we introduce **exterior product** $\wedge$ for its image:
$$a(v_{1}\otimes v_{2}\otimes \cdots\otimes v_{n})=v_{1}\wedge v_{2}\wedge \cdots\wedge v_{n}$$
such that $v \wedge v=0 ,\forall v\in V$. One can verify that the image of $a$ is a [[Vector Subspace|subspace]], denoted by $\bigwedge^{n}V$. Based on this, we can generalize the exterior product to $\wedge:\bigwedge^{p}V\times \bigwedge^{q}V\to\bigwedge^{p+q}V$ as
$$(v_{1}\wedge \cdots\wedge v_{p})\wedge(w_{1}\wedge \cdots\wedge w_{q})=v_{1}\wedge \cdots\wedge v_{p}\wedge w_{1}\wedge \cdots\wedge w_{q}.$$

The **exterior algebra** $\bigwedge V=\bigoplus_{n=1} \bigwedge^{n}V$ equipped with exterior product is an [[Associative Algebra|associative algebra]]. It satisfies:
1. *anti-symmetry*: $\forall v,w\in  V, v\wedge w=-w\wedge v$.
2. *graded anti-symmetry*: $\forall v\in \bigwedge^{p}V,w\in \bigwedge^{q}V,v\wedge w=(-1)^{pq}w\wedge v$.