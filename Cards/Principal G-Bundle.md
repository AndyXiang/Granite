---
tags:
  - Area/Math/Topology/FiberBundle
  - Area/Math/Algebra/Group
---
Let $G$ be a [[Topological Group|topological group]]. The [[Fiber Bundle|fiber bundle]] $(E,B,G,\pi)$ is called a **principal $G$-bundle** as:
1. The total space $E$ has a fiberwise [[Group Action#Basic concepts|free right action]] $\mu:E\times G\to E$ as the diagram commutes
```tikz
\usepackage{tikz-cd}
\begin{document}
	\begin{tikzcd}
		E\times G \ar[r, "\mu"] \ar[d, "\pi\times 1"'] & E \ar[d, "\pi"] \\
		B\times \{1\} \ar[r, "\mathrm{proj}"] & B
	\end{tikzcd}
\end{document}
```
2. The induced action on fibers $$\mu: \pi ^{-1}(x)\times G\to \pi ^{-1}(x)$$ is free and [[Group Action#Basic concepts|transitive]].
3. The local trivializations $\phi: \pi ^{-1}(U)\to U\times G$ are [[Group Action#Basic concepts|equivariant]], that is, the diagram commutes
```tikz
\usepackage{tikz-cd}
\begin{document}
	\begin{tikzcd}
		\pi^{-1}(U)\times G \ar[r, "\phi\times \mathrm{id}", leftrightarrow] \ar[d, "\mu"] & U\times G\times G \ar[d, "\mathrm{id}\times \mathrm{mul}"] \\
		\pi^{-1}(U) \ar[r, "\phi", leftrightarrow] & U\times G
	\end{tikzcd}
\end{document}
```

 
