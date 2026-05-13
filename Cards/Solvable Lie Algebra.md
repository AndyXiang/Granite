---
tags:
  - Area/Math/Algebra/LieAlgebra
---
Let $\mathfrak{g}$ be a [[Lie Algebra|Lie algebra]] over [[Field (Math)|field]] $\mathbb{K}$. Define the series of [[Lie Ideal|ideals]] $\mathfrak{g}^{(k)},k\in \mathbb{N}$ by $\mathfrak{g}^{(0)}=\mathfrak{g}$ and 
$$\mathfrak{g}^{(k+1)}=[\mathfrak{g}^{(k)},\mathfrak{g}^{(k)}].$$
The Lie algebra is **solvable** if $\mathfrak{g}^{(n)}=0$ for some $n\in \mathbb{N}$.

## Representations of solvable Lie algebras
>[!tip] Lie's theorem about representations of solvable Lie algebra
>Let $\pi:\mathfrak{g}\to \mathfrak{gl}(V)$ be a complex [[Representation (Lie Algebra)|representation]] of a solvable Lie algebra $\mathfrak{g}$. Then there exists a basis in $V$ s.t. in this basis, $\forall x\in \mathfrak{g}$, $\pi(x)$ is upper-triangular.

This theorem is a generalization of a well-known result that any operator in a complex [[Vector Space|vector space]] can be brought to an upper-triangular form by a change of basis.