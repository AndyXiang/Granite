---
tags:
  - Area/Math/Topology/FiberBundle
---
Similar to the idea of [[Differential Manifold|differential manifold]], which locally looks like [[Euclidean Space|Euclidean space]], the idea of **fiber bundle** is a [[Topological Space|topological space]] that locally looks like a product of two other topological spaces.

A **fiber bundle** (or **local trivial fiber bundle**) is the data $(E,B,F,\pi)$ as:
1. A topological space $E$ called the **total space**.
2. A topological space $B$ called the **base space**.
3. A topological space $F$ called the **fiber**.
4. A [[Map#Properties|surjection]] $\pi:E\to B$ satisfying $\pi ^{-1}(p)\cong F$, called the **projection space**. The inverse image $\pi ^{-1}(p)=F_{p}$ is called the fiber at $p\in B$.
5. For every point $x\in B$ there is an [[Topological Space|open neighborhood]] $U\subset B$ and a [[Homeomorphism|homeomorphism]] $\phi: \pi ^{-1}(U)\to U\times F$, called the **local trivialization**, that makes the diagram commutes:
```tikz
\usepackage{tikz-cd}
\begin{document}
	\begin{tikzcd}
		\pi^{-1}(U) \ar[r, "\phi", leftrightarrow] \ar[d, "\pi"] & U\times F \ar[d, "\mathrm{proj}"]\\
		U \ar[r, equal] & U
	\end{tikzcd}
\end{document}
```

This definition can be generalized with extra structure over the three topological spaces.

## Transition functions
For a set of open [[Covering Space|covering]] $\{ U_{i} \}$ of $B$, the local trivializations on the intersection $U_{i}\cap U_{j}$ induce a homeomorphism $t_{ij}:(U_{i}\cap U_{j})\times F\to (U_{i}\cap U_{j})\times F$ as
$$t_{ij}=\phi_{j}^{-1}\circ \phi_{i}.$$
This is called the **transition function**.



## Morphism of fiber bundles
A [[Morphism|morphism]] of fiber bundles $\Phi:(E,B,F,\pi)\to(E',B',F',\pi')$ is a pair of [[Continuous Map (Topology)|continuous maps]] $\phi_{1}:E\to E'$ and $\phi_{2}:B\to B'$ making the diagram commutes:
```tikz
\usepackage{tikz-cd}
\begin{document}
	\begin{tikzcd}
		E \ar[r, "\phi_1"] \ar[d, "\pi"] & E' \ar[d, "\pi'"]\\
		B \ar[r, "\phi_2"] & B'
	\end{tikzcd}
\end{document}
```
These two also define the continuous map $\phi_{3}:F\to F'$ by restriction. A [[Isomorphism|isomorphism]] of fiber bundles is such morphism with inverse.


## Section
For a fiber bundle $(E,B,F,\pi)$, a **section** $s:B\to E$ is a [[Continuous Map (Topology)|continuous mapping]] which satisfies $s \circ\pi =\mathrm{id}_{B}$. This is also called a **global section**. For $U\subset B$, one may define a **local section** $s:U\to E$. Note that not all fiber bundles admit global sections.