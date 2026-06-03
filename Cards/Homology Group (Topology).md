---
tags:
  - Area/Math/Topology/Homology
  - Area/Math/Category/AdditiveCategory/AbelianCategory/Homology
---
## Of chain complexes
Let $K$ be a $n$-dimensional [[Simplex|simplicial simplex]] and $C_{r}(K)$ be its [[Chain Complex & Cochain complex|chain group]]. The [[Chain Complex & Cochain complex|boundary operator]] $\partial_{r}$ is a map $C_{r}(K)\to C_{r-1}(K)$.

The kernel of $\partial_{r}$ is a [[Subgroup|subgroup]] of chain group
$$Z_{r}(K)=\mathrm{ker}(\partial _{r})\lhd C_{r}(K).$$
Its elements are called **$r$-cycles**. Also the image:
$$B_{r}(K)=\mathrm{img}(\partial _{r+1}) \lhd C_{r}(K)$$
whose elements are called **$r$-boundaries**. One can proves that $B_{r}(K)\lhd Z_{r}(K)$ by proving $\partial_{r}\circ \partial_{r+1}=0$.

The **$r$th homology group** $H_{r}(K)$ for $0\leq r\leq n$ is defined by
$$H_{r}(K)=Z_{r}(K)/ B_{r}(K).$$

## Properties
1. Homology groups are [[Z Topological Invariant|topological invariants]].
2. Let $K$ be a [[Connected Space|connect]] simplicial complex, then $H_{0}(K)\cong \mathbb{Z}$.
3. Let $K$ be a disjoint union of $N$ [[Connected Space|connected components]], that is $K=K_{1} \cup \cdots\cup K_{N}, K_{i}\cap K_{j}=\varnothing$. Then $$H_{r}(K)=H_{r}(K_{1}) \oplus \cdots\oplus  H_{r}(K_{N}).$$
