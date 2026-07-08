---
tags:
  - Area/Math/Category
---
Let $\mathbf{C}$ be a [[Category|category]] and $f:x\to y$ one of its morphism. $f$ is a **monomorphism** iff $\forall z\in \mathrm{ob}(\mathbf{C})$ and $g_{1},g_{2}:z\to x$, the diagram
```tikz
\usepackage{tikz-cd}
\begin{document}
	\begin{tikzcd}
			z \ar[r, bend left,"g_1"] \ar[r, bend right,"g_2"'] & x \ar[r,"f"] & y
	\end{tikzcd}
\end{document}
```
commutes, i.e. $f\circ g_{1}=f \circ g_{2}\Leftrightarrow g_{1}=g_{2}$.

Specifically, one use the notation
$$f:x \hookrightarrow y$$
for monomorphisms.

