---
tags:
  - Area/Math/Category
---
Let $\mathbf{C}$ be a [[Category|category]] with [[Initial Object|initial object]] $i$. The **kernel** of [[Morphism|morphism]] $f:x\to y$ is the morphism $\mathrm{ker}(f):k\to x$ such that the morphisms $k\to i$ exists and
```tikz
\usepackage{tikz-cd}
\begin{document}
	\begin{tikzcd}
		z \ar[r, "\exists !h"] \ar[rd, "g"] & k \ar[r] \ar[d,"\mathrm{ker}(f)"] & i \ar[d]\\
		& x \ar[r, "f"] & y
	\end{tikzcd}
\end{document}
```
commutes.

Let $\mathbf{C}$ be a [[Category|category]] with [[Terminal Object|terminal object]] $t$. The **cokernel** of [[Morphism|morphism]] $f:x\to y$ is the morphism $\mathrm{coker}(f):y\to q$  such that the morphisms $t\to\mathrm{coker}(f)$ exist sand
```tikz
\usepackage{tikz-cd}
\begin{document}
	\begin{tikzcd}
		x \ar[r, "f"] \ar[d] & y \ar[d, "\mathrm{coker}(f)"'] \ar[dr, "g"] & \\
		t \ar[r] & q \ar[r, "\exists !h"] & z
	\end{tikzcd}
\end{document}
```
commutes.