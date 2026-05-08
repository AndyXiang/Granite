---
tags:
  - Area/Math/Algebra/Group
---
Let $G,N$ be [[Group|groups]], and $\alpha:G\to \mathrm{aut}(N)$ be a [[Homomorphism (Group)|group homomorphism]]. The **semidirect product** $N\rtimes_{\alpha}G$ is the [[Cartesian Product|Cartesian product]] $N\times G$ equipped with the binary operation
$$(n,h)(n',h')=(n\alpha(h)n',hh'),\forall n,n'\in N,h,h'\in H.$$

The identity is $(1,1)$, while inverse is $(n,h)^{-1}=(\alpha(h^{-1})n^{-1},h^{-1})$. Apparently $N$ is [[Normal Subgroup|normal subgroup]] of $N\rtimes H$.

>[!note] Lemma
>Let $G$ be a group and $N,H$ be its subgroups, while $H \subset \mathrm{stab}(N)$. Define $\alpha:H\to \mathrm{aut}(N)$ as $\alpha(h)(n)=hnh^{-1}$. Then
> $$\mu:\begin{matrix}
  N \rtimes_{\alpha} H &\to & G  \\
(n,h) & \to & nh
\end{matrix}$$
> is a group homomorphism. $\mu$ is [[Isomorphism|isomorphism]] iff $NH=G$ and $N \cap H=\{ 1 \}$.



## Examples
1. The [[Dihedral Group|dihedral group]] $\mathrm{D}_{n}$ is the semidirect product of $\mathbb{Z}_{2}$ and $\mathbb{Z}_{n}$, with the homomorphism $\alpha:\mathbb{Z}_{2}\to \mathrm{aut}(\mathbb{Z}_{n})$ defined by $\alpha(x):y\mapsto-y$ for $x\in \mathbb{Z}_{2},y\in \mathbb{Z}_{n}$.
