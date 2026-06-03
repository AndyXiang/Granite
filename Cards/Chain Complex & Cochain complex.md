---
tags:
  - Area/Math/Category/AdditiveCategory/AbelianCategory
---
Let $\mathbf{A}$ be an [[Additive Category|additive category]]. A **chain complex** $X_{\bullet}$ is a [[Complex|complex]]
$$\dots\to x_{n+1}\xrightarrow{d_{n+1}}x_{n} \xrightarrow{d_{n}}x_{n-1}\to \dots$$
where $\forall n\in \mathbb{Z}$, $x_{n}\in \mathrm{ob}(\mathbf{A})$, $d_{n}\in \mathrm{mor}_{\mathbf{A}}(x_{n+1},x_{n})$ such that $d_{n}\circ d_{n+1}=0$.

A [[Morphism|morphism]] of chain complexes $f:X_{\bullet}\to Y_{\bullet}'$ is a family of morphisms $f_{n}:x_{n}\to y_{n}$ such that
```tikz
\usepackage{tikz-cd}
\begin{document}
	\begin{tikzcd}
		x_n \ar[r, "d_n"] \ar[d, "f_n"] & x_{n-1} \ar[d, "f_{n-1}"] \\ 
		y_n \ar[r, "d'_n"] & y_{n-1} 
	\end{tikzcd}
\end{document}
```
commutes.

The [[Category|category]] of chain complexes is denoted $\mathbf{Ch}(\mathbf{A})$. This category is abelian.

A **cochain complex** $X^{\bullet}$ is a [[Complex|complex]]
$$\dots\to x^{n-1}\xrightarrow{d^{n-1}}x^{n} \xrightarrow{d^{n}}x^{n+1}\to \dots$$
where $\forall n\in \mathbb{Z}$, $x^{n}\in \mathrm{ob}(\mathbf{A})$, $d^{}{n}\in \mathrm{mor}_{\mathbf{A}}(x^{n},x^{n+1})$ such that $d^{n+1}\circ d^{n}=0$.

A [[Morphism|morphism]] of cochain complexes $f:X^{\bullet}\to Y^{\bullet}$ is a family of morphisms $f_{n}:x_{n}\to y_{n}$ such that
```tikz
\usepackage{tikz-cd}
\begin{document}
	\begin{tikzcd}
		x^n \ar[r, "d^n"] \ar[d, "f^n"] & x^{n+1} \ar[d, "f^{n+1}"] \\ 
		y^n \ar[r, "d^n"] & y^{n+1} 
	\end{tikzcd}
\end{document}
```
commutes.

The category of cochain complexes is denoted $\mathbf{Coch}(\mathbf{A})$. This category is abelian.