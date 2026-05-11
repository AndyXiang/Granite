---
tags:
  - Area/Math/Algebra/LieAlgebra
---
Let $\mathfrak{g}$ be a finite-dimensional [[Lie Algebra|Lie algebra]] over [[Field (Math)|field]] $\mathbb{K}$. A **Killing form** $B:\mathfrak{g}\times \mathfrak{g}\to \mathbb{K}$ is the symmetric bilinear form given by
$$B(x,y)=\mathrm{tr}(\mathfrak{ad}(x)\circ\mathfrak{ad}(y)),x,y\in \mathfrak{g}$$
where $\mathfrak{ad}:\mathfrak{g}\to \mathrm{aut}(\mathfrak{g})$ is the [[Adjoint Action|adjoint action]].

Let $x_{i},i=1,2,\cdots,n$ be the basis of $\mathfrak{g}$. The Killing form can be written as
$$B(x_{i},x_{j})=C_{ik}^{~~~~l}C_{jl}^{~~~k}.$$


## Properties
1. Killing form is *invariant*: $B(x,[y,z])=B([x,y],z)$.
2. $\mathfrak{g}$ is [[Solvable Lie Algebra|solvable]] iff $B(x,y)=0$ for every $x\in[\mathfrak{g},\mathfrak{g}]$ and $y\in \mathfrak{g}$.
3. $\mathfrak{g}$ is [[Simple Lie Algebra|semisimple]] iff $B(x,y)$ is non-degenerate.