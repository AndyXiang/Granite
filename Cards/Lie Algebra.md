---
tags:
  - Area/Math/Algebra/Group/LieGroup
  - Area/Math/Algebra/LieAlgebra
---
A **Lie algebra** over [[Field (Math)|field]] $\mathbb{K}$ is is a [[Vector Space|vector space]] $\mathfrak{g}$ over $\mathbb{K}$ with a $\mathbb{K}$-bilinear [[Map|map]] $[-,-]:\mathfrak{g}\times \mathfrak{g}\to \mathfrak{g}$, called the **commutator**, satisfying:
1. *skew-symmetric*: $\forall x,y\in \mathfrak{g},[x,y]=-[y,x]$.
2. *Jacobi identity*: $\forall x,y,z\in \mathfrak{g},[x,[y,z]]+[y,[z,x]]+[z,[x,y]]=0$.

A **[[Morphism|morphism]] of Lie algebra** is a $\mathbb{K}$-linear map $f:\mathfrak{g}_{1}\to \mathfrak{g}_{2}$ which preserves the commutator.

>[!tip] Theorem
>For any real or complex finite-dimensional Lie algebra $\mathfrak{g}$, there is a unique (up to isomorphism) [[Connected Space|connected]] and [[Connected Space|simply connected]] Lie group $G$ that $T_{1}G=\mathfrak{g}$. Any other connected Lie group $G'$ with Lie algebra $\mathfrak{g}$ must be of the form $G /Z$ for some discrete [[Center (Group)|central]] [[Subgroup|subgroup]] $Z\lhd G$. 

In short, the above theorem states the [[Equivalent Category|equivalence]] between the [[Category|category]] of Lie algebras and the category of connected simply-connected Lie groups.
## Related
1. [[Z Simple Lie Algebra|Simple Lie algebra and semisimple Lie algebra]].
2. [[Z Reductive Lie Algebra|Reductive Lie algebra]].