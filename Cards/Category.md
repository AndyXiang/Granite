---
tags:
  - Area/Math/Category
---
**Category theory** is a theory of mathematical structure and general relations. A category $\mathbf{C}$ is defined with three data:
1. a class $\mathrm{ob}(\mathbf{C})$, called *objects* of $\mathbf{C}$.
2. a class $\mathrm{mor}(\mathbf{C})$, that contains map between objects, called *morphisms* of $\mathbf{C}$. Morphisms are defined with *domain* and *codomain*. There must be an *identity morphism $\mathrm{id}_{x}$* for every object $x$, i.e. $\forall x\in \mathrm{ob}(\mathbf{C}),\exists \mathrm{id}_{x}\in \mathrm{mor}(\mathbf{C}),x \xrightarrow{\mathrm{id}_{x}}x$.
3. a *composition rule* for morphisms, such that whenever the codomain of a morphism $f$ matches the domain of a morphism $g$, there is a morphism $g\circ f$ called their composition. The composition is associative: $h\circ(g\circ f)=(h\circ g)\circ f$ and unital: $\mathrm{id}\circ f=f\circ\mathrm{id}=f$.

```tikz
\usepackage{tikz-cd}
\begin{document}
	\begin{tikzcd}
		&&&\\
		w \ar[r,"f"] \ar[rr, bend left=50, "g\circ f"] \ar[loop left, "\mathrm{id}_w"]& x  \ar[r,"g"] \ar[rr, bend right=50, "h\circ g"] & y  \ar[r, "h"] & z  \ar[loop right, "\mathrm{id}_z"]\\
		&&&
	\end{tikzcd}
\end{document}
```
