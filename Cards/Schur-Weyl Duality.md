---
tags:
  - Area/Math/Algebra/Group/LieGroup/GeneralLinearGroup
  - Area/Math/Algebra/Group/PermutationGroup
  - Area/Math/Representation
---
**Schur-Weyl duality**, also called Frobenius-Schur duality, is a relation between finite-dimensional [[Irreducible Representation|irreducible]] [[Linear Representation|linear representations]] of [[General Linear Group|general linear group]] $\mathrm{GL}(k)$ and the [[Permutation Group|permutation group]] $S_{n}$.

Concretely, for $k,n\in \mathbb{N}$ consider the [[Direct Product (Vector Space)|tensor product]] of $n$ copies of $k$-dimensional [[Vector Space|vector space]] $\mathbb{C}^{k}$ as a $k\times n$-dimensional vector space: $\otimes^{n}\mathbb{C}^{k}$. As such, this carries:
1. a canonical linear representation of $\mathrm{GL}(k,\mathbb{C})$ as the $n$-fold [[Product Representation|product]] of its [[Fundamental Representation|fundamental representation]] on $\mathbb{C}^{k}$.
2. a canonical linear representation of $S_{n}$ given by permutation of the $n$ tensor factors.
The statement of Schur-Weyl duality is that this linear representation for the [[Direct Product (Group)|product group]] $\mathrm{GL}(n,\mathbb{C})\times S_{n}$ decomposes as a [[Direct Sum|direct sum]] of products of irreducible representations for either group, as follows:
$$\otimes ^{n}\mathbb{C}^{k}\cong \bigoplus _{\lambda \vdash n,l(\lambda)\leq k}D^{(\lambda)}\otimes S^{(\lambda)}$$
where $\lambda$ is a [[Partition|partition]] of $n$ with $k$ cells. $D^{(\lambda)}$ is the irreducible [[Polynomial Representation|polynomial representation]] of $\mathrm{GL}(n,\mathbb{C})$ labeled by $\lambda$, and $S^{(\lambda)}$ is the [[Specht Module|Specht module]] of $S_{n}$ also labeled by $\lambda$.
