---
tags:
  - Area/Math/Category
---
Let $\mathbf{C}$ be a [[Category|category]] with [[Initial Object|initial object]] $i$. The **kernel** of [[Morphism|morphism]] $f:x\to y$ is the morphism $\mathrm{ker}(f)\to x$ such that the morphisms $\mathrm{ker}(f)\to i$ exists and
```tikz
\usepackage{tikz-cd}
\begin{document}
	\begin{tikzcd}
		\mathrm{ker}(f) \ar[r] \ar[d,""] & i \ar[d]\\
		x \ar[r, "f"] & y
	\end{tikzcd}
\end{document}
```
commutes.

Let $\mathbf{C}$ be a [[Category|category]] with [[Terminal Object|terminal object]] $t$. The **cokernel** of [[Morphism|morphism]] $f:x\to y$ is the morphism $y\to \mathrm{coker}(f)$  such that the morphisms $t\to\mathrm{coker}(f)$ exist sand
```tikz
\usepackage{tikz-cd}
\begin{document}
	\begin{tikzcd}
		x \ar[r, "f"] \ar[d] & y \ar[d]\\
		t \ar[r] & \mathrm{coker}(f) 
	\end{tikzcd}
\end{document}
```
commutes.