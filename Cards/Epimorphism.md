---
tags:
  - Area/Math/Category
---
Let $\mathbf{C}$ be a [[Category|category]] and $f:x\to y$ one of its [[Morphism|morphism]]. $f$ is a **epimorphism** iff $\forall z\in \mathrm{ob}(\mathbf{C})$ and $g_{1},g_{2}:z\to x$, the diagram
```tikz
\usepackage{tikz-cd}
\begin{document}
	\begin{tikzcd}
		 x \ar[r,"f"] & y \ar[r, bend left,"g_1"] \ar[r, bend right,"g_2"'] & z
	\end{tikzcd}
\end{document}
```
commutes, i.e. $g_{1}\circ f=g_{2}\circ f \Leftrightarrow g_{1}=g_{2}$.

Specifically, one use the notation
$$f:x \twoheadrightarrow  y$$
for epimorphisms.
