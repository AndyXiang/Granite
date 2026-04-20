---
tags:
  - Area/Math/Algebra/LieAlgebra
  - Area/Math/Algebra/AssociativeAlgebra
---
Let $\mathfrak{g}$ be a [[Lie Algebra|Lie algebra]] over a [[Field (Math)|field]] $\mathbb{K}$. The **universal enveloping algebra** of $\mathfrak{g}$, denoted by $U(\mathfrak{g})$, is the [[Quotient Algebra|quotient algebra]] $T(\mathfrak{g}) /(xy-yx-[x,y]),x,y\in \mathfrak{g}$, where $T(\mathfrak{g})$ is the [[Tensor Algebra|tensor algebra]] of $\mathfrak{g}$.

>[!tip] Universality
>Let $A$ be an [[Associative Algebra|associative algebra]] with unit over $\mathbb{K}$ and let $\rho:\mathfrak{g}\to A$ be a linear map s.t. $\rho(x)\rho(y)-\rho(y)\rho(x)=\rho([x,y])$. Then $\rho$ can be uniquely extended to a [[Morphism|morphism]] of associative algebras $U(\mathfrak{g})\to A$.

As a corollary, any [[Representation|representation]] of $\mathfrak{g}$ is a $U(\mathfrak{g})$-[[Module|module]].

With [[Poincaré-Birkhoff-Witt Theorem|Poincaré-Birkhoff-Witt theorem]], one finds that the map $\mathfrak{g}\mapsto U(\mathfrak{g})$ is injective.